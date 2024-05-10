# Project Responsive Web Design using Bootstrap
## Date:

## AIM:
To design a responsive website for a Pharmaceutical Company using Bootstrap.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
```
<html>
    <head>
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title> Product Page </title>
        {%load static%}
        <style type="text/css">
            * {
                margin: 0;
                padding: 0;
                font-family: Arial, Helvetica, sans-serif;
            }
            .banner {
                width: 100%;
                height: 100vh;
                background-image: linear-gradient(rgba(0,0,0,0.75),rgba(0,0,0,0.75)),url(background.jpg);
                background-size: cover;
                background-position: center;
            }
            .navbar {
                width: 85%;
                margin: auto;
                padding: 35px 0;
                display: flex;
                align-items: center;
                justify-content: space-between;
            }
            body {
                background: -webkit-linear-gradient(bottom, #2dbd6e, #a6f77b);
                background-repeat: no-repeat;
            }
            .bg-product {
                border: 1px;
                padding: 10px;
                color: white;
                background-color: #6fa1f8;
                border-radius: 30px;
            }
            .logo {
                color: #6fa1f8;
                font-size: 30px;
                font-weight: 700;
                letter-spacing: 1px;
            }
            span {
                color: white;
            }
            form {
                width: 300px;
                height: 40px;
                display: flex;
                background: rgba(255, 255, 255, 0.2);
                padding: 1px 1px;
                font-size: 15px;
                border-radius: 10px;
                backdrop-filter: blur(4px) saturate(180%);
            }
            form input {
                background: transparent;
                flex: 1;
                border: 0;
                outline: none;
                padding: 12px 20px;
                font-size: 15px;
                color: white;
            } 
            ::placeholder {
                color: white;
            }
            form button {
                border: 0;
                outline: none;
                padding: 5px 20px;
                color: white;
                border-radius: 10px;
                background: #6fa1f8;
                cursor: pointer;
            }
            .navbar li {
                list-style: none;
                display: inline-block;
                margin: 0 20px;
                position: relative;
            }
            .navbar li a {
                text-decoration: none;
                color: white;
                text-transform: uppercase;
            }
            .navbar li:hover {
                border: 1px;
                padding: 10px;
                color: white;
                background-color: #6fa1f8;
                transition: 0.5s; 
                cursor: pointer;
                border-radius: 30px;
            }
            .container {
                background: transparent;
                padding: 10px 5%;
                padding-bottom: 100px;
            }
            .container .box-container {
                display: grid;
                grid-template-columns: repeat(auto-fit, minmax(170px, 1fr));
                gap: 20px;
            }
            .container .box-container .box {
                color: white;
                box-shadow: 0 5px 10px rgba(0,0,0,.2);
                border-radius: 20px;
                background: transparent;
                border: 1px solid white;
                padding: 20px 10px;
            }
            .container .box-container .box img {
                height: 40px;
                border-radius: 10px;
            }
            .container .box-container .box h3 {
                color: #6fa1f8;
                font-size: large;
                padding: 10px 0;
            }
            .container .box-container .box p {
                color: white;
                font-size: small;
                line-height: 1.5;
            }
            footer {
                background-color: #6fa1f8;
                margin-top: auto;
            }
        </style>
    </head>
<body>
    <div class="banner">
        <br>
        <div class="navbar">
            <h1 class="logo">C<span>ode</span>C<span>rafters</span></h1>
            <ul>
                <li><a href="http://127.0.0.1:8000/"> Home </a></li>
                <li><a href="http://127.0.0.1:8000/product" class="bg-product"> Products </a></li>
                <li><a href="http://127.0.0.1:8000/people"> People </a></li>
                <li><a href="http://127.0.0.1:8000/contact"> Contact </a></li>
            </ul>
            <form action="" method="get">
                <input type="text" placeholder="Enter to Search">
                <button type="submit"> Search </button>
            </form>
        </div>
        <div class="container">
            <div class="box-container">
                <div class="box">
                    <img src="{% static 'logo2.png' %}" alt="">
                    <h3> SiteGenie Builder </h3>
                    <p> Simplified drag and drop website creation. </p>
                </div>
                <div class="box">
                    <img src="{% static 'logo3.png' %}" alt="">
                    <h3> DevSync Hub Pro </h3>
                    <p> Efficient version control and sync. </p>
                </div>
                <div class="box">
                    <img src="{% static 'logo4.png' %}" alt="">
                    <h3> CodeLeap Toolkit </h3>
                    <p> Tools for innovative web development. </p>
                </div>
                <div class="box">
                    <img src="{% static 'logo9.png' %}" alt="">
                    <h3> Comtug Software </h3>
                    <p> Robust multi-layered website security. </p>
                </div>
                <div class="box">
                    <img src="{% static 'logo6.png' %}" alt="">
                    <h3> WebFlow Pro Studio </h3>
                    <p> Rapid low-code app creation. </p>
                </div>
                <div class="box">
                    <img src="{% static 'logo10.png' %}" alt="">
                    <h3> Norton Toolkit </h3>
                    <p> Automated testing and debugging. </p>
                </div>
                <div class="box">
                    <img src="{% static 'logo8.png' %}" alt="">
                    <h3> Teamm Code </h3>
                    <p> Streamlined code content management. </p>
                </div>
                <div class="box">
                    <img src="{% static 'logo11.png' %}" alt="">
                    <h3> WideFix </h3>
                    <p> Optimized code correcting tools. </p>
                </div>
                <div class="box">
                    <img src="{% static 'logo12.png' %}" alt="">
                    <h3> Datatech eSolutions </h3>
                    <p> Optimized code efficiency tools. </p>
                </div>

                <div class="box">
                    <img src="{% static 'logo13.png' %}" alt="">
                    <h3> World Soft </h3>
                    <p> Seamless high-traffic handling. </p>
                </div>
                <div class="box">
                    <img src="{% static 'logo14.png' %}" alt="">
                    <h3> MINDTECH </h3>
                    <p> Integrated tools for developers. </p>
                </div>
            </div>
        </div>
    </div>
    <footer>
        <center>Designed by : Naveen Kumar V (212223220068) </center>
    </footer>
</body>
</html>
```
## OUTPUT:
<img width="892" alt="product" src="https://github.com/NaveenKumarV2005/Pharma/assets/151476286/51ad550d-f266-4f27-845e-bf3d98f8f928">

## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
