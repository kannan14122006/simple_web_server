# EX01 Developing a Simple Webserver

# Date:30/11/2024
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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LAPTOP SPECIFICATONS</title>
   <style>
        body {
            font-family: Arial, sans-serif;
            background-color: lightgreen;
          
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        .specs-container {
            border: 2px;
            border-color: black;
            background-color:whitesmoke;
            padding: 20px;
            border-radius: 7px;
            box-shadow:whitesmoke;
            width: 800px;
        }
        h1 {
            text-align: center;
            color:red;
        }
        table {
            width: 100%;
            border-collapse: collapse;
        }
        th, td {
            padding: 5px;
            text-align: left;
            border-bottom: 1px solid rgb(165, 158, 158);
        }
        th {
            background-color: #c3c5cb;
        }
        .brand{
            
            font-weight: 600;
        }
        nav{
            border: 5px;
        }
        .top{
            word-spacing: 20PX;
            font-family: "Bokor", system-ui;
            font-size: xx-large;
        }
    </style>
</head>
<body>
    <div class="specs-container">
        <nav>
        <h1 class="top">LAPTOP SPECIFICATONS</h1>
        </nav>
        <table>
           
            <tr>
                <td style="font-weight: 700;">Brand</td>
                <td CLASS="brand">LENOVO</td>
                
            </tr>
            <tr>
                <td style="font-weight: 700;">Model</td>
                <td>ThinkPad E16 Gen 1</td>
            </tr>
            <tr>
                <td style="font-weight: 700;">Processor</td>
                <td>13th Gen Intel(R) Core(TM) i5-1335U   1.30 GHz</td>
            </tr>
            <tr>
                <td style="font-weight: 700;">Display</td>
                <td>16inch Full HD</td>
            <tr>
                <td style="font-weight: 700;">Operating System</td>
                <td>Windows 11 Home Single Language</td>
            </tr>
            <tr>
                <td style="font-weight: 700;">System Type</td>
                <td>64-bit operating system, x64-based processor</td>
            </tr>
            <tr>
                <td style="font-weight: 700;">RAM</td>
                <td>16 GB (15.7 GB usable)</td>
            </tr>
            <tr>
                <td style="font-weight: 700;">Storage</td>
                <td>350 GB  SSD</td>
            </tr>
            <tr>
                <td style="font-weight: 700;">Graphics</td>
                <td>NVIDIA GeForce MX 550</td>
            </tr>
            
            </tr>
            <tr>
                <td style="font-weight: 700;">Battery Life</td>
                <td>5 to 8 hours</td>
            </tr>
            <tr>
                <td style="font-weight: 700;">Charging Capacity</td>
                <td>68 Watt</td>
            </tr>
            
            <tr>
                <td style="font-weight: 700;">Price</td>
                <td>Rs: 55000 </td>
            </tr>
        </table>
    </div>
</body>
</html>
```
# OUTPUT:
![Screenshot 2024-12-06 102233](https://github.com/user-attachments/assets/e3b4933f-3f70-448a-acf5-d9ccee5b848d)


# RESULT:
The program for implementing simple webserver is executed successfully.
