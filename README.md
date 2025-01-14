<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SF BEN Clone</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
        }
        body {
            background-color: #f9f9f9;
        }
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
            border-bottom: 2px solid #ccc;
        }
        header .logo {
            font-size: 24px;
            font-weight: bold;
        }
        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: #333;
        }
        .tabs {
            margin: 20px;
        }
        .tabs button {
            padding: 10px 20px;
            margin-right: 10px;
            border: none;
            background-color: #eee;
            cursor: pointer;
        }
        .tabs button.active {
            background-color: #6a0dad;
            color: white;
        }
        .content {
            display: flex;
            justify-content: space-between;
            margin: 20px;
        }
        .article {
            width: 65%;
            background-color: white;
            padding: 20px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        .sidebar {
            width: 30%;
        }
        .sidebar img {
            width: 100%;
            margin-bottom: 20px;
        }
        .play-button {
            position: relative;
            display: inline-block;
        }
        .play-button::before {
            content: '\25B6';
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 48px;
            color: rgba(255, 255, 255, 0.8);
        }
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0,0,0,0.8);
            justify-content: center;
            align-items: center;
        }
        .modal img {
            width: 60%;
        }
        .close {
            position: absolute;
            top: 20px;
            right: 40px;
            font-size: 40px;
            color: white;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">SF BEN</div>
        <nav>
            <a href="#">Events</a>
            <a href="#">Career</a>
            <a href="#">AppAssessor</a>
            <a href="#">Salesforce News</a>
            <a href="#">Articles by Role</a>
        </nav>
    </header>

    <div class="tabs">
        <button class="active">Latest</button>
        <button>Most Popular</button>
        <button>Editors' Picks</button>
    </div>

    <div class="content">
        <div class="article">
            <h1>Are Salesforce </h1>
            <h1>Certifications Still</h1>
            <h1> Relevant?Top Voices Join </h1>
            <h1>the Great Cert Debate</h1>
            <p>By Henry Martin - January 10, 2025</p>
            <div class="play-button" onclick="openModal()">
                <img src="C:\Users\shilp\Downloads\Telegram Desktop\skull_image_placeholder.jpg" alt="Colorful Skull" width="200%">
            </div>
        </div>
        <div class="sidebar">
            <img src="C:\Users\shilp\Downloads\Telegram Desktop\ad1_placeholder.jpg" alt="Ad 1" width = "75%">
            <img src="C:\Users\shilp\Downloads\Telegram Desktop\ad2_placeholder.jpg" alt="Ad 2" width = "75%">
        </div>
    </div>

    <div class="modal" id="imageModal">
        <span class="close" onclick="closeModal()">&times;</span>
        <img src="C:\Users\shilp\Downloads\Telegram Desktop\skull_image_placeholder.jpg" alt="Colorful Skull Enlarged">
    </div>

    <script>
        function openModal() {
            document.getElementById('imageModal').style.display = 'flex';
        }

        function closeModal() {
            document.getElementById('imageModal').style.display = 'none';
        }
    </script>
</body>
</html>
