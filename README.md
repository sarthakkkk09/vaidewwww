# vaidewwww
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Expressing Feelings to Vaidehi</title>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap">
    <style>
        body {
            background-color: #f4e8db;
            color: #333;
            font-family: 'Pacifico', cursive, sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
        }

        #container {
            padding: 30px;
            background-color: rgba(255, 255, 255, 0.9);
            border-radius: 15px;
            margin: 50px auto;
            width: 80%;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        #clock {
            font-size: 32px;
            margin-bottom: 20px;
        }

        #message {
            font-size: 24px;
            margin-bottom: 20px;
            border: 2px solid #2196F3;
            padding: 20px;
            border-radius: 15px;
        }

        #heartDivider {
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 20px 0;
        }

        #heartIcon {
            width: 30px;
            height: 30px;
            fill: #e91e63;
            margin: 0 10px;
        }

        #dateIdeas {
            margin-top: 20px;
            font-size: 20px;
        }

        #options {
            display: flex;
            justify-content: center;
            margin-top: 20px;
        }

        button {
            padding: 15px 30px;
            margin: 0 15px;
            font-size: 20px;
            cursor: pointer;
            background-color: #e91e63;
            color: #fff;
            border: none;
            border-radius: 10px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.2);
        }
    </style>
</head>
<body>
    <div id="container">
        <div id="clock"></div>
        <div id="message">
            <p>Dear Vaidehi,</p>
            <p>From the moment our paths crossed, my heart has been captivated by your warmth and kindness. I find myself smiling at the thought of you. The sparkle in your eyes is like a beacon of joy. Would you do me the honor of going on a date with me? I believe our connection is something special, and I would love the chance to get to know you better.</p>
        </div>
        <div id="heartDivider">
            <svg id="heartIcon" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                <path d="M12 21.35l-1.45-1.32C6.4 15.36 2 12.28 2 8.5 2 5.42 4.42 3 7.5 3c1.74 0 3.41.81 4.5 2.09C15.09 3.81 16.76 3 18.5 3 21.58 3 24 5.42 24 8.5c0 3.78-4.4 6.86-8.55 11.54L12 21.35z"/>
            </svg>
        </div>
        <div id="dateIdeas">
            <label for="dateOptions">Choose a date idea:</label>
            <select id="dateOptions">
                <option value="vrExperience">Virtual Reality Experience</option>
                <option value="foodTruckAdventure">Food Truck Adventure</option>
                <option value="escapeRoom">Escape Room Challenge</option>
                <option value="outdoorPicnic">Outdoor Picnic and Stargazing</option>
                <option value="DIYCrafting">DIY Crafting Session</option>
                <option value="concertNight">Concert Night</option>
                <option value="beachGetaway">Beach Getaway</option>
                <option value="movieMarathon">Movie Marathon at Home</option>
                <option value="artGallery">Art Gallery Exploration</option>
                <option value="cookingClass">Cooking Class Together</option>
                <option value="karaokeNight">Karaoke Night</option>
                <option value="hikingAdventure">Hiking Adventure</option>
                <option value="comedyShow">Comedy Show Date</option>
                <option value="historicalTour">Historical Site Tour</option>
                <option value="spaDay">Relaxing Spa Day</option>
                <option value="hotAirBalloonRide">Hot Air Balloon Ride</option>
                <option value="zooVisit">Zoo Visit</option>
                <option value="danceClass">Dance Class Experience</option>
            </select>
        </div>
        <div id="options">
            <button onclick="alert('Great choice! Looking forward to our date!')">Yes</button>
            <button onclick="redirectToHome()">No</button>
        </div>
    </div>

    <script>
        function updateClock() {
            const now = new Date();
            const hours = now.getHours().toString().padStart(2, '0');
            const minutes = now.getMinutes().toString().padStart(2, '0');
            const seconds = now.getSeconds().toString().padStart(2, '0');
            document.getElementById('clock').textContent = `Current time: ${hours}:${minutes}:${seconds}`;
        }

        function redirectToHome() {
            window.location.href = 'home.html'; /* Replace 'home.html' with your actual home page URL */
        }

        setInterval(updateClock, 1000);
        updateClock();
    </script>
</body>
</html>
