# Ex.08 Design of Interactive Image Gallery
## Date:07/05/2025

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :

filename.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title>
    <link rel="stylesheet" href="style.css">
</head>
<body bgcolor="#fcefee">
    <header>
        <h1 align="center">ANIME</h1>
    </header>
    <div class="gallery1">
        <div class="gallery-item" onclick="openModal(this)">
            <img src="solo-leveling-.jpg" >
        </div>
        <div class="gallery-item" onclick="openModal(this)">
            <img src="naruto.avif"  >
        </div>
    </div>
        <div class="gallery2">
            <div class="gallery-item" onclick="openModal(this)">
                <img src="black clover.jpeg" >
            </div>
            <div class="gallery-item" onclick="openModal(this)">
                <img src="jujutsukaisen.jpg" >
            </div>
        </div>

    <div id="modal" class="modal">
        <span class="close" onclick="closeModal()">&times;</span>
        <img class="modal-content" id="modalImage">
        <div id="caption"></div>
    </div>

    <script src="style.js"></script>
</body>
</html>
```
style.js

```
function openModal(element) {
    const modal = document.getElementById("modal");
    const modalImage = document.getElementById("modalImage");
    const caption = document.getElementById("caption");

    modal.style.display = "flex";
    modalImage.src = element.querySelector("img").src;
    caption.textContent = element.querySelector("img").alt;
}

function closeModal() {
    const modal = document.getElementById("modal");
    modal.style.display = "none";
}
```
style.css

```
img{
    width: 250px;
    height: 200px;
    object-fit: cover;
    display: flex;
    border-radius: 10px;

}
.gallery1,.gallery2{
    display: flex;
    justify-content: center;
    gap: 40px;
    margin-top: 20px;
}
```



## OUTPUT:

![alt text](<Screenshot 2025-05-07 111838.png>)

![alt text](<Screenshot 2025-05-07 111902.png>)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
