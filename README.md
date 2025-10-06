# Ex.08 Design of Interactive Image Gallery
# Date:06.10.2025
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
````
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   
    <body>
        <header>
            <h1 style="color: yellow;">TOP ANIME</font></h1>
        </header>
        <header>
            <h2 style="color: yellow;">2025</font></h2>
        </header>
    </body>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-color: #f4f4f4;
             background-image: url("Screenshot 2025-10-06 204333.png");
            background-size:cover;
        }

        h1 {
            margin-top: 20px;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            padding: 20px;
        }

        .gallery img {
            width: 300px;
            height: 200px;
            border: 2px solid #ccc;
            border-radius: 8px;
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
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .modal img {
            max-width: 90%;
            max-height: 90%;
            border: 4px solid white;
            border-radius: 10px;
        }

        .modal span {
            position: absolute;
            top: 20px;
            right: 40px;
            font-size: 30px;
            color: white;
            cursor: pointer;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1 style="color: yellow;">Interactive Photo Gallery Done by ASHWIN BAALAJI V K (25011987)</h1>
    <div class="gallery">
        <img src="Screenshot 2025-10-06 202724.png" alt="Image 1" onclick="openModal(this)">
        <img src="Screenshot 2025-10-06 202930.png" alt="Image 2" onclick="openModal(this)">
        <img src="Screenshot 2025-10-06 203139.png" alt="Image 3" onclick="openModal(this)">
        <img src="Screenshot 2025-10-06 203357.png" alt="Image 4" onclick="openModal(this)">
        <img src="Screenshot 2025-10-06 203433.png" alt="Image 5" onclick="openModal(this)">
        <img src="Screenshot 2025-10-06 203523.png" alt="Image 5" onclick="openModal(this)">
        <img src="Screenshot 2025-10-06 203655.png" alt="Image 5" onclick="openModal(this)">
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
</body>
</html>



````
# OUTPUT:
<img width="1910" height="1040" alt="Screenshot 2025-10-06 221807" src="https://github.com/user-attachments/assets/ca196f27-c871-4967-b1f7-9b122168b01e" />
<img width="1898" height="1038" alt="Screenshot 2025-10-06 221914" src="https://github.com/user-attachments/assets/a1e79120-260e-4576-baf6-489e9fa60cbe" />
<img width="1884" height="1040" alt="Screenshot 2025-10-06 221948" src="https://github.com/user-attachments/assets/2d3c60ab-2e7e-484d-ba93-86398cc55445" />
<img width="1904" height="1038" alt="Screenshot 2025-10-06 222013" src="https://github.com/user-attachments/assets/844b013f-b9a8-4d7a-9653-1519177d5d2d" />
<img width="1898" height="1038" alt="Screenshot 2025-10-06 222035" src="https://github.com/user-attachments/assets/58a8cd88-0b2a-4373-b282-c14329c245a8" />
<img width="1913" height="1039" alt="Screenshot 2025-10-06 222055" src="https://github.com/user-attachments/assets/82d5a8df-bf57-44eb-8835-1dcdb787a132" />
<img width="1914" height="1040" alt="Screenshot 2025-10-06 222120" src="https://github.com/user-attachments/assets/3809a05c-a782-4e53-b2bd-479abc043d34" />
<img width="1909" height="1038" alt="Screenshot 2025-10-06 222144" src="https://github.com/user-attachments/assets/879f03fa-e785-4f17-bdce-3b80777729b2" />
<img width="1909" height="1040" alt="Screenshot 2025-10-06 222226" src="https://github.com/user-attachments/assets/08a30f72-dfab-4968-bdfc-068487f28329" />









# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
