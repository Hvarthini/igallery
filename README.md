# Ex.08 Design of Interactive Image Gallery
## Date:27.05.25

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
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ART GALLERY</title>
    <style>
        body {
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-color: rgb(248, 235, 220);
            background-size: cover;  
            background-position: center;
            background-attachment: fixed;   
            background-repeat: no-repeat;
        }

        h1 {
            margin-top: 20px;
            font-family:cursive;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            padding: 10px;
        }

        .gallery img {
            width: 350px;
            height: 250px;
            border: 6px solid #000000;
            border-radius: 30px;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.1);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(120, 147, 156, 0.8);
            justify-content: center;
            align-items: center;
        }

        .modal img {
            max-width: 90%;
            max-height: 90%;
            border: 4px solid rgb(1, 1, 1);
            border-radius: 30px;
        }

        .modal span {
            position: absolute;
            top: 20px;
            right: 40px;
            font-size: 50px;
            color: rgb(0, 0, 0);
            cursor: pointer;
            font-weight: bold;
        }
        footer{
            font-size: xx-large;

        }
    </style>
</head>
<body>
    <h1>ART GALLERY</h1>
    <div class="gallery">
        <img src="niagara.jpg" alt="Image 1" onclick="openModal(this)">
        <img src="airballoon.jpeg" alt="Image 2" onclick="openModal(this)">
        <img src="northern light.jpeg" alt="Image 3" onclick="openModal(this)">
        <img src="lantern.jpeg" alt="Image 4" onclick="openModal(this)">
        <img src="greek.jpg" alt="Image 5" onclick="openModal(this)">
        <img src="italy.jpeg" alt="Image 1" onclick="openModal(this)">
        <img src="bioluminescent.jpeg" alt="Image 2" onclick="openModal(this)">
        <img src="bridge.webp" alt="Image 3" onclick="openModal(this)">
        <img src="maldives.jpg" alt="Image 4" onclick="openModal(this)">
        <img src="paris.jpeg" alt="Image 5" onclick="openModal(this)">
    </div>
    <div class="modal" id="imageModal">
        <span onclick="closeModal()">&times;</span>
        <img id="modalImage" src="" alt="">
    </div>
    <script>
        function openModal(image) {
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');
            modal.style.display = 'flex';
            modalImg.src = image.src;
        }
        function closeModal() {
            const modal = document.getElementById('imageModal');
            modal.style.display = 'none';
        }
    </script>
    <footer> <p>B.Harshavarthini 212224110023</p></footer>
</body>
</html>
~~~
## OUTPUT:
![image](https://github.com/user-attachments/assets/d30cefa3-485d-4efd-b790-738ea07cae3e)
![image](https://github.com/user-attachments/assets/7bbb1131-a648-4218-82a9-a4e7f389fc73)
![image](https://github.com/user-attachments/assets/1fa23fbd-af73-4900-906b-d7e348bf30a6)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
