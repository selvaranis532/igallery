# Ex.08 Design of Interactive Image Gallery
## Date:21.12.2024

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
    <title>GALLERY OF BRAVE QUEEN</title>
    <style>
        body {
            font-family: sans-serif;
            background-color: pink;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            flex-direction: column;
        }

        .gallery-container {
            text-align: center;
            width: 50%;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }

        .gallery-item {
            width: 150px;
            height: 150px;
            transition: transform 0.3s ease;
            cursor: pointer;  
        }

        footer {
            text-align: center;
            font-size: 28px;
            margin-top: 70px;
        }
    </style>
</head>
<body>
    <div class="gallery-container">
        <h1>GALLERY OF SAMANTHA</h1>
        <div class="gallery">
            <img src="image1.jpg" alt="Image 1" class="gallery-item" id="sam1" onclick="zoomInOut('sam1')">
            <img src="image2.jpg" alt="Image 2" class="gallery-item" id="sam2" onclick="zoomInOut('sam2')">
            <img src="image3.jpg" alt="Image 3" class="gallery-item" id="sam3" onclick="zoomInOut('sam3')">
            <img src="image4.jpg" alt="Image 4" class="gallery-item" id="sam4" onclick="zoomInOut('sam4')">
            <img src="image5.jpg" alt="Image 5" class="gallery-item" id="sam5" onclick="zoomInOut('sam5')">
            <img src="image6.jpg" alt="Image 6" class="gallery-item" id="sam6" onclick="zoomInOut('sam6')">
            <img src="image7.jpg" alt="Image 7" class="gallery-item" id="sam7" onclick="zoomInOut('sam7')">
            <img src="image8.jpg" alt="Image 8" class="gallery-item" id="sam8" onclick="zoomInOut('sam8')">
        </div>
    </div>
    <footer>
        Designed and Developed By Selvarani
    </footer>

    <script>
        function zoomInOut(imageId) {
            var image = document.getElementById(imageId);
            if (image.style.transform === "scale(2)") {
                image.style.transform = "scale(1)";  
            } else {
                image.style.transform = "scale(2)";  
            }
        }
    </script>
</body>
</html>
```
## OUTPUT:
![alt text](<1 (2).png>)
![alt text](<2 (2).png>)
## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
