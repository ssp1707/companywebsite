# Web Design for a Manufacturing Company
## AIM: 
To design a static website for a chip manufacturing company.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Updating the sample content.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.

## PROGRAM:

### base.html
```
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <title> CODE Industries Limited </title>
    <link rel="stylesheet" href="{% static 'css/layout.css' %}">
    <link rel="icon" href="{% static 'img/starkicon.jpg' %}" type="image/x-icon">

</head>

<body>
    <div class="container">
        <div class="banner">
            CODE Industries Limited
        </div>
        <div class="menu">
            <div class="menuitem"><a href="/home">Home</a></div>
            <div class="menuitem"><a href="/products">Products</a></div>
            <div class="menuitem"><a href="/people">People</a></div>
            <div class="menuitem"><a href="/contactus">Contact Us</a></div>
        </div>
        <div class="content">
            {% block content %}
            {% endblock  %}
        </div>
        <div class="footer">
            Copyright © 2021 CODE Industries Limited, Developed by Emma Watson
        </div>
    </div>
</body>

</html>


```

### home.html
```
{% extends "website/base.html" %}

{% block content %}
<div class="homecontent">
    <h1>About Us</h1>
    <img src="/static/img/Building.jpg" alt="Building">
    <div class="contenttext">
        STARK Industries Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications that
        serve the data center, networking, software, broadband, wireless, and storage and industrial markets. Common
        applications for its products include: data center networking, home connectivity, broadband access,
        telecommunications equipment, smartphones, base stations, data center servers and storage, factory automation,
        power generation and alternative energy systems, displays, and mainframe operations and management, and
        application software development. Some of Silicon's core technologies and products include:
        <ul>
            <li>Memory Chips</li>
            <li>SATA HDD</li>
            <li>SATA SSD </li>
            <li>Broadband Modems</li>
            <li>Wifi Devices</li>
            <li>Switching Devices</li>
            <li>Optical Sensors</li>
        </ul>
    </div>
</div>
{% endblock  %}
```
### products.html
```
{% extends "website/base.html" %}

{% block content %}
<div class="productcontent">
    <h1>Our Premium Products</h1>
    <div class="productitems">
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/c1.jpeg" alt="product image">
            </div>
            <div class="itemname">4GB DDRA4 laptop memory</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/c2.jpg" alt="product image">
            </div>
            <div class="itemname">1TB Laptop HDD</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/graphic card.png" alt="product image">
            </div>
            <div class="itemname">Graphic card</div>
            <div class="itemprice">Price: Rs.30000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/mouse.jpg" alt="product image">
            </div>
            <div class="itemname">mouse</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/speaker.webp" alt="product image">
            </div>
            <div class="itemname">speaker</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/ram rgb.jpg" alt="product image">
            </div>
            <div class="itemname">ram rgb</div>
            <div class="itemprice">Price: Rs.4000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/RGB Keyboard.jpg" alt="product image">
            </div>
            <div class="itemname">RGB Keyboard</div>
            <div class="itemprice">Price: Rs.2500.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/SATA SSD.jpg" alt="product image">
            </div>
            <div class="itemname">SATA SSD (samsung)</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/Boom Headset.jpg" alt="product image">
            </div>
            <div class="itemname">Boom Headset</div>
            <div class="itemprice">Price: Rs.3000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/pendrive.jpg" alt="product image">
            </div>
            <div class="itemname">pendrive 64gb</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/iot-board.jpg" alt="product image">
            </div>
            <div class="itemname">iot-board</div>
            <div class="itemprice">Price: Rs.5500.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/processor.jpg" alt="product image">
            </div>
            <div class="itemname">intel i9 9900k processor</div>
            <div class="itemprice">Price: Rs.36000.00 </div>
        </div>
    </div>
</div>
{% endblock  %}
```
### people.html
```
{% extends "website/base.html" %}

{% block content %}
<div class="peoplecontent">
    <h1>Our Crew</h1>
    <div class="crewmembers">
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/emma.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">EMMA WATSON</div>
            <div class="designation">C.E.O AK CORP</div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/daniel.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">DANIEL RADCLIFFE</div>
            <div class="designation">COO</div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/will.webp" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">WILL SMITH</div>
            <div class="designation">TECHNICAL TEAM</div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/jessica.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">JESSICA ALBA</div>
            <div class="designation"> R & D HEAD </div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/brie.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">BRIE LARSON</div>
            <div class="designation"> DESIGN TEAM </div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/ellen.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">ELLEN DEGENREOUS</div>
            <div class="designation"> MARKETING HEAD </div>
        </div>
    </div>
    {% endblock  %}
```
### contactus.html
```
{% extends "website/base.html" %}

{% block content %}
<form action="//submit.form" id="ContactUs100" method="post" onsubmit="return ValidateForm(this);">
    <script type="text/javascript">
        function ValidateForm(frm) {
            if (frm.Name.value == "") { alert('Name is required.'); frm.Name.focus(); return false; }
            if (frm.FromEmailAddress.value == "") { alert('Email address is required.'); frm.FromEmailAddress.focus(); return false; }
            if (frm.FromEmailAddress.value.indexOf("@") < 1 || frm.FromEmailAddress.value.indexOf(".") < 1) { alert('Please enter a valid email address.'); frm.FromEmailAddress.focus(); return false; }
            if (frm.Comments.value == "") { alert('Please enter comments or questions.'); frm.Comments.focus(); return false; }
            return true;
        }
    </script>
    <table style="width:100%;max-width:550px;border:0;" cellpadding="8" cellspacing="0">
        <tr>
            <td>
                <label for="Name">Name*:</label>
            </td>
            <td>
                <input name="Name" type="text" maxlength="60" style="width:100%;max-width:250px;" />
            </td>
        </tr>
        <tr>
            <td>
                <label for="PhoneNumber">Phone number:</label>
            </td>
            <td>
                <input name="PhoneNumber" type="text" maxlength="43" style="width:100%;max-width:250px;" />
            </td>
        </tr>
        <tr>
            <td>
                <label for="FromEmailAddress">Email address*:</label>
            </td>
            <td>
                <input name="FromEmailAddress" type="text" maxlength="90" style="width:100%;max-width:250px;" />
            </td>
        </tr>
        <tr>
            <td>
                <label for="Comments">Comments*:</label>
            </td>
            <td>
                <textarea name="Comments" rows="7" cols="40" style="width:100%;max-width:350px;"></textarea>
            </td>
        </tr>
        <tr>
            <td>
                * - required fields
            </td>
            <td>
                <input name="skip_Submit" type="submit" value="Submit" />
            </td>
        </tr>
    </table>
</form>
{% endblock  %}
```

## OUTPUT:
![output](./static/img/output1.PNG)

![output](./static/img/output2.PNG)

![output](./static/img/output3.PNG)

![output](./static/img/output4.PNG)

![output](./static/img/output5.PNG)

![output](./static/img/output6.PNG)

## CODE VALIDATION REPORT:
![output](./static/img/report1.PNG)

![output](./static/img/report2.PNG)

![output](./static/img/report3.jpeg)

![output](./static/img/report4.jpeg)

![output](./static/img/report5.jpeg)
## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://sanjnapriya.student.saveetha.in:8000/. HTML code is validated.