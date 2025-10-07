# Ex.08 Design of Interactive Image Gallery
## Date:

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
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title>
    <style>
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 16px;
            padding: 1rem;
            max-width: 800px;
            margin: 0 auto;
        }
        .gallery-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <header style="text-align: center; background-color: #333; color: white; padding: 1rem 0;">
        <h1>IMAGE GALLERY (GALAXY)</h1>
    </header>

    <div class="gallery-grid">
        <div class="gallery-item" onclick="openModal(this)">
            <img src="1.jpg">
        </div>
        <div class="gallery-item" onclick="openModal(this)">
            <img src="2.webp">
        </div>
        <div class="gallery-item" onclick="openModal(this)">
            <img src="3.webp">
        </div>
        <div class="gallery-item" onclick="openModal(this)">
            <img src="4.avif">
        </div>
        <div class="gallery-item" onclick="openModal(this)">
            <img src="5.webp">
        </div>
        <div class="gallery-item" onclick="openModal(this)">
            <img src="6.jpg">
        </div>
        <div class="gallery-item" onclick="openModal(this)">
            <img src="7.jpg">
        </div>
    </div>

    <div id="modal" style="display: none; position: fixed; z-index: 1; left: 0; top: 0; width: 100%; height: 100%; background-color: rgba(0,0,0,0.9);">
        <span style="position: absolute; top: 15px; right: 35px; color: white; font-size: 40px; font-weight: bold; cursor: pointer;" onclick="closeModal()">&times;</span>
        <img id="modalImage" style="display: block; margin: 5% auto; max-width: 80%;">
    </div>

    <script>
        function openModal(element) {
            var modal = document.getElementById("modal");
            var modalImg = document.getElementById("modalImage");
            modal.style.display = "block";
            modalImg.src = element.querySelector("img").src;
        }

        function closeModal() {
            document.getElementById("modal").style.display = "none";
        }
    </script>
</body>
</html>
```
## OUTPUT:
![alt text](1.jpg)
![alt text](2.webp)
![alt text](3.webp)
![alt text](4.avif)
![alt text](5.webp)
![alt text](6.jpg)
![alt text](7.jpg)



## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
