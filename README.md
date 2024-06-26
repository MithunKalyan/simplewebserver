# EX01 Developing a Simple Webserver
## Date:
29.03.2024
## AIM:
To develop a simple webserver to serve html pages.

## DESIGN STEPS:
### Step 1: 
HTML content creation.

### Step 2:
Design of webserver workflow.

### Step 3:
Implementation using Python code.

### Step 4:
Serving the HTML pages.

### Step 5:
Testing the webserver.

## PROGRAM:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        h1{
            color: green;
            text-align: center;
        }
.topnav {
  overflow: hidden;
  background-color: #333;
  position: relative;
}
.topnav #myLinks {
  display: none;
}
.topnav a {
  color: white;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
  display: block;
}
.topnav a.icon {
  background: black;
  display: block;
  position: absolute;
  right: 0;
  top: 0;
}
.topnav a:hover {
  background-color: #ddd;
  color: black;
}
.active {
  background-color: #04AA6D;
  color: white;
}
.centre {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 8%;
  text-align: center;
  margin-top: 0%;
}
h5{
    color: green;
}
    </style>
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
</head>
<body style="background-color: black;">
    <h1 style="color: green;">Welcome to Zoro!!</h1>
 <div>
    <img src="https://qph.cf2.quoracdn.net/main-qimg-a8d54c56b627ffa411e158354ce2a22c" alt="" class="centre">
 </div>
    <!-- Load an icon library to show a hamburger menu (bars) on small screens -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

<!-- Top Navigation Menu -->
<div class="topnav">
  <a href="#home" class="active">Home</a>
  <!-- Navigation links (hidden by default) -->
  <div id="myLinks">
    <a href=>Subbed Anime</a>
    <a href=>Dubbed Anime</a>
    <a href=>Most Popular</a>
    <a href=>Movies</a>
    <a href=>TV Series</a>
    <a href=>Search</a>
  </div>
  <!-- "Hamburger menu" / "Bar icon" to toggle the navigation links -->
  <a href="javascript:void(0);" class="icon" onclick="myFunction()">
    <i class="fa fa-bars"></i>
  </a>
</div>
 <script>
    function myFunction() {
  var x = document.getElementById("myLinks");
  if (x.style.display === "block") {
    x.style.display = "none";
  } else {
    x.style.display = "block";
  }
}
 </script> <br />
 <div id="carouselExampleDark" class="carousel carousel-dark slide">
    <div class="carousel-indicators">
      <button type="button" data-bs-target="#carouselExampleDark" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
      <button type="button" data-bs-target="#carouselExampleDark" data-bs-slide-to="1" aria-label="Slide 2"></button>
      <button type="button" data-bs-target="#carouselExampleDark" data-bs-slide-to="2" aria-label="Slide 3"></button>
    </div>
    <div class="carousel-inner">
      <div class="carousel-item active" data-bs-interval="10000">
        <img src="https://imgsrv.crunchyroll.com/cdn-cgi/image/format=auto,width=1200,height=675,fit=contain,quality=85/catalog/crunchyroll/a249096c7812deb8c3c2c907173f3774.jpe" class="d-block w-100" alt="...">
        <div class="carousel-caption d-none d-md-block">
          <h5 style="color: white;">One Piece</h5>
          <p style="color: white;">#1 trending today</p>
        </div>
      </div>
      <div class="carousel-item" data-bs-interval="2000">
        <img src="https://www.dexerto.com/cdn-cgi/image/width=3840,quality=75,format=auto/https://editors.dexerto.com/wp-content/uploads/2023/09/10/solo-leveling-anime-poster.jpeg" class="d-block w-100" alt="...">
        <div class="carousel-caption d-none d-md-block">
          <h5 style="color:white;" >Solo Leveling</h5>
          <p style="color: white;">#2 trending today</p>
        </div>
      </div>
      <div class="carousel-item">
        <img src="https://staticg.sportskeeda.com/editor/2023/08/d83bc-16929832322856-1920.jpg?w=840" class="d-block w-100" alt="...">
        <div class="carousel-caption d-none d-md-block">
          <h5 style="color: white;">Classroom of the Elite</h5>
          <p style="color: white;">#3 trending today</p>
        </div>
      </div>
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleDark" data-bs-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleDark" data-bs-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </button>
  </div>
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
</body>
</html>
## OUTPUT:
![alt text](<Screenshot 2024-03-26 160426.png>)

## RESULT:
The program for implementing simple webserver is executed successfully.
