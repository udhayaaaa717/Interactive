# Ex.08 Design of Interactive Image Gallery
## Date:07.10.25

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
        <h1>IMAGE GALLERY (MAHENDRA SIGN DHONI)</h1>
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
<img width="1920" height="1058" alt="Screenshot 2025-10-07 153122" src="https://github.com/user-attachments/assets/d8a21bf1-8f1d-4103-9131-6ed2dc1ed326" />
<img width="1920" height="1095" alt="Screenshot 2025-10-07 154350" src="https://github.com/user-attachments/assets/33071eec-d834-493a-8b0f-e756f1075fce" />
<img width="1914" height="1095" alt="Screenshot 2025-10-07 153152" src="https://github.com/user-attachments/assets/e3e34af3-6158-4237-9047-e2738f9f0c3e" />
<img width="1920" height="1097" alt="Screenshot 2025-10-07 153203" src="https://github.com/user-attachments/assets/e535be1b-2e14-4004-996b-cd5cf844df10" />
<img width="1920" height="1095" alt="Screenshot 2025-10-07 153216" src="https://github.com/user-attachments/assets/de42cc80-8a2f-4011-8a9c-a420069828db" />
<img width="1920" height="1095" alt="Screenshot 2025-10-07 153228" src="https://github.com/user-attachments/assets/97a00265-3809-4eef-8333-dd684bd32cea" />
<img width="1906" height="1092" alt="Screenshot 2025-10-07 153242" src="https://github.com/user-attachments/assets/3c904fd7-e459-45bc-9c99-24e0425f01a8" />








## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
