# EX01 Developing a Simple Webserver

# Date:06/12/2024
# AIM:
To develop a simple webserver to serve html pages and display the configuration details of laptop.

# DESIGN STEPS:
## Step 1:
HTML content creation.

## Step 2:
Design of webserver workflow.

## Step 3:
Implementation using Python code.

## Step 4:
Serving the HTML pages.

## Step 5:
Testing the webserver.

# PROGRAM:
```
from http.server import HTTPServer,BaseHTTPRequestHandler
content='''
<!DOCTYPE html>
<html>
<head>
<title>My Web Server</title>
<style>
table{
color: white;
font-weight: 500;
border-radius: 9px;
border-color: red;
}
tr,th,td{
border-radius: 5px;
}
td{
font-size: 15px;
}
.name{
color: black;
}
</style>
</head>
<body>
<table border="1" bgcolor="black" align="center"cellpadding="20" >
<caption class="name">LAPTOP CONFIGURATION</caption>
<tr>
<th>SYSTEM CONFIGURATION</th>
<th>DESCRIPTION</th>
</tr>
<tr>
<td>Operating System</td>
<td>Windows 11</td>
</tr>
<tr>
<td>Manufacturer</td>
<td>Lenovo</td>
</tr>
<tr>
<td>Processor</td>
<td>13th Gen Intel(R) Core(TM) i5-1335U 1.30 GHz</td>
</tr>
<tr>
<td>RAM</td>
<td>16.0GB</td>
</tr>
<tr>
<td>Secondary Memory</td>
<td>512GB</td>
</tr>
</table>
</body>
</html>
'''
class MyServer(BaseHTTPRequestHandler):
    def do_GET(self):
        print("Get request received...")
        self.send_response(200)
        self.send_header("content-type", "text/html")
        self.end_headers()
        self.wfile.write(content.encode())
print("This is my webserver")
server_address =('',8000)
httpd = HTTPServer(server_address,MyServer)
httpd.serve_forever()
```

# OUTPUT:
![Screenshot 2024-12-06 154245](https://github.com/user-attachments/assets/5116b357-90c2-4b13-8ef6-ae2a1016d205)
![Screenshot 2024-12-06 154309](https://github.com/user-attachments/assets/1d4a567f-a49f-40a1-bc03-fa2011c91455)


# RESULT:
The program for implementing simple webserver is executed successfully.
