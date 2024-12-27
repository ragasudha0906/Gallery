# Ex.08 Design of Interactive Image Gallery
# Date:16-11-2024
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html>
<head>
    <meta name="viewport" content="width=device-width , initial-scale=1.0">
    <title>Image Gallery</title>
    <link rel="stylesheet" href="image gallery.css">
</head>
<body>
    <div class="full-img" id="fullImgBox">
        <img src="img gallery-1.jpg" id="fullImg">
        <span onclick="closeFullImg()">X</span>
    </div>

    <div class="img-gallery">
        <img src="c:\Users\admin\Downloads\snowman.webp" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Downloads\elephant.webp" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Downloads\lighting images.jpg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Downloads\house.jpg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Downloads\cat.avif" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Downloads\falls.jpg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Downloads\adventure.webp" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Downloads\dolphin.webp" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Downloads\moon.jpg" onclick="openFullImg(this.src)">
    </div>

<script>
    var fullImgBox = document.getElementById("fullImgBox");
    var fullImg = document.getElementById("fullImg");

    function openFullImg(pic){
        fullImgBox.style.display="flex";
        fullImg.src = pic;
    }

    function closeFullImg(){
        fullImgBox.style.display="none";

    }
</script>
</body>
</html>
*{
    margin: 0;
    padding: 0;
    font-family:sans-serif;
}
body{
    background: #ecf4fb;
}
.img-gallery{
    width: 70%;
    margin: 100px auto 50px;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px,1fr));
    grid-gap:30px;
}
.img-gallery img{
    width: 100%;
    height: 100%;
    cursor:pointer;
}
.img-gallery img:hover{
    transform: scale(0.8) rotate(-25deg);
    border-radius: 20px;
    box-shadow: 0 32px 75px rgba(68,77,136,0.2);

}
.full-img{
    width: 100%;
    height: 100vh;
    background: rgba(0,0,0,0.9);
    position: fixed;
    top: 0;
    left: 0;
    display: none;
    align-items: center;
    justify-content: center;
    z-index: 100;

}
.full-img img{
    width: 90%;
    max-width: 500px;
}
.full-img span{
    position: absolute;
    top: 5%;
    right: 5%;
    font-size: 30px;
    color: #fff;
    cursor:pointer;

}
```
# OUTPUT:
![Screenshot 2024-12-27 210910](https://github.com/user-attachments/assets/ebaa4341-677b-4adc-879b-5ecee45a9e9f)
![snow 1](https://github.com/user-attachments/assets/ed89d25a-189a-46ac-8566-ab4ee6fc4808)
![elephant 1](https://github.com/user-attachments/assets/78f45666-7862-4c7f-8d2e-f02855f2559e)
![nature 1](https://github.com/user-attachments/assets/d0b3d6ef-d8d9-44b4-9c7e-9fb377dd4d12)
![lighting 1](https://github.com/user-attachments/assets/f972d6b0-f7a8-4afd-b04c-86b7defda965)
![cat 1](https://github.com/user-attachments/assets/a983fdcd-55c8-4ff6-8d38-9af1973acbc6)
![falls](https://github.com/user-attachments/assets/ee28e7a1-bdd5-462a-b1a1-97e5c9c03aaa)
![Screenshot 2024-12-27 211913](https://github.com/user-attachments/assets/4bfb3903-4b5f-4f88-9e56-966f22e1650e)
![Screenshot 2024-12-27 211939](https://github.com/user-attachments/assets/2857a2c2-f2d2-4ebc-82c3-67b7da9832ba)

# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
