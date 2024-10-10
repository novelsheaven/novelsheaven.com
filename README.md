<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title>Novels Heaven - PDF Downloads</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background-color: #F4F4F4;
            color: #333;
        }

        .container {
            width: 80%;
            margin: 0 auto;
        }

        header {
            background-color: #333;
            color: #E0E0E0;
            padding: 20px 0;
            text-align: center;
        }

        .logo {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 15px;
        }

        header h1 {
            font-size: 3em;
            margin-bottom: 10px;
        }

        header p {
            font-size: 1.2em;
        }

        .header-flex {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 10px;
        }

        .social-icons {
            display: flex;
            gap: 10px;
        }

        .social-icons img {
            width: 30px;
            height: 30px;
        }

        .date-time {
            font-size: 14px;
            color: #333;
        }

        .downloads-section {
            padding: 50px 0;
            background-color: #fff;
        }

        .downloads-section h2 {
            text-align: center;
            font-size: 2.5em;
            margin-bottom: 30px;
        }

        .novel-list {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
        }

        .novel-item {
            background-color: #eee;
            padding: 20px;
            margin: 10px;
            border-radius: 10px;
            width: 200px;
            text-align: center;
        }

        .novel-item h3 {
            font-size: 1.2em;
            margin-bottom: 10px;
        }

        .novel-item img {
            width: 100%;
            height: auto;
            border-radius: 5px;
            margin-bottom: 10px;
        }

        .novel-item p {
            font-size: 1em;
            color: #555;
            margin-bottom: 10px;
        }

        .novel-item a {
            display: inline-block;
            padding: 10px 20px;
            background-color: #333;
            color: #fff;
            border-radius: 5px;
            text-decoration: none;
        }

        .novel-item a:hover {
            background-color: #555;
        }

        footer {
            background-color: #333;
            color: #E0E0E0;
            padding: 20px 0;
            text-align: center;
        }

        footer p {
            margin: 0;
        }
    </style>
</head>
<body>
    <header>
        <div class="container header-flex">
            <!-- Left: Social Media Links -->
            <div class="social-icons">
                <a href="https://www.tiktok.com/@farisghaazi_7?is_from_webapp=1&sender_device=pc" target="_blank">
                    <img src="https://i.ibb.co/X5wrLWp/1553127754.png" alt="TikTok">
                </a>
                <a href="https://www.instagram.com/" target="_blank">
                    <img src="https://i.ibb.co/jWn6fz8/15707869.png" alt="Instagram">
                </a>
                <a href="https://www.youtube.com/" target="_blank">
                    <img src="https://i.ibb.co/XSWkcvv/logo-youtube-video-icon-18.png" alt="YouTube">
                </a>
            </div>

            <!-- Center: Logo and Title -->
            <div class="logo-title">
                <img src="https://i.ibb.co/rMFkRbc/ce5f5e88-0eab-4a9a-81a6-479f72a93ce6.jpg" alt="Novels Heaven Logo" class="logo">
                <h1>Novels Heaven</h1>
                <p>Explore and Download Urdu Novels in PDF</p>
            </div>

            <!-- Right: Date and Time -->
            <div id="datetime" class="date-time"></div>
        </div>
    </header>

    <section class="downloads-section">
        <div class="container">
            <h2>Available Novels for Download</h2>
            <div class="novel-list">
                <!-- Example novel -->
                <div class="novel-item">
                    <h3>Episode 1: Novel Title</h3>
                    <img src="images/novel1.jpg" alt="Novel 1 Image">
                    <p>Author: Author Name</p>
                    <a href="pdfs/novel1.pdf" download>Download PDF</a>
                </div>
                <!-- More novels can be added here -->
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2024 Novels Heaven. All rights reserved.</p>
        </div>
    </footer>

    <!-- JavaScript for Date and Time -->
    <script>
        function updateDateTime() {
            const now = new Date();
            const options = { 
                weekday: 'long', 
                year: 'numeric', 
                month: 'long', 
                day: 'numeric', 
                hour: '2-digit', 
                minute: '2-digit', 
                second: '2-digit', 
                hour12: true 
            };
            const dateTimeString = now.toLocaleDateString('en-US', options);
            document.getElementById('datetime').innerHTML = dateTimeString;
        }

        setInterval(updateDateTime, 1000); // Update the date and time every second
        updateDateTime(); // Initial call to display the time right away
    </script>
</body>
</html>


