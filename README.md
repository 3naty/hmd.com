<!DOCTYPE html>
<html lang="ar">
<head>

<!DOCTYPE html>
<html>
<head>
    <title>HMD</title>
</head>
<body>
<script>
    var names = [
        { name: "[ hmd ]", color: "red" },
        { name: "[ hmd ]", color: "white" }
    ];

    var nameIndex = 0;

    function changeNames() {
        var currentName = names[nameIndex];
        document.getElementById("name").textContent = currentName.name;
        document.getElementById("name").style.color = currentName.color;
        nameIndex = (nameIndex + 1) % names.length;
    }

    // Change the names every 1 second
    setInterval(changeNames, 1000);
</script>
<p align="center">
    <img border="0" src="https://cdn.discordapp.com/attachments/1241104301049516104/1241104473372233809/d8847891b8119de9.png?ex=664b9f1d&is=664a4d9d&hm=833573b81d64a9ad37bd9f116a7d868f1fba22230d1ca0758f8ceeb3db1252ef&">
</p>
<p align="center">
    <font face="Courier" size="6" style="color: #000000;">
        <span style="color: rgb(255, 0, 0);">Hacked By</span>
        <span id="name"></span>
    </font>
</p>
<p align="center">
    <b>
<font face="Courier" color="#000000">
<a href="https://discord.gg/R56" style="font-size: 24px; color: rgb(255, 255, 255); text-decoration: none;">Discord.gg/R56</a>



</font>

    </b>
</p>
</body>
</html>
<!DOCTYPE html>
<html>
<head>
    <title>Panadol Store</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            color: #000000;
            background-color: #000000;
            overflow: hidden;
        }

        h1, h3 {
            color: #ffffff;
        }

        #ip-address {
            color: rgb(255, 255, 255);
        }

        #ip-info {
            font-family: Arial, sans-serif;
            white-space: pre;
            color: rgb(255, 255, 255);
        }

        .cmd-text-container {
            position: relative;
        }

        .cmd-text {
            color: #000000;
            font-size: 9px;
            font-family: Arial, sans-serif;
            white-space: nowrap;
            position: absolute;
            animation: scrollText 20s linear infinite;
            transform: translateX(100%);
            -webkit-text-stroke: 1px rgb(255, 255, 255);
            text-stroke: 1px rgb(255, 255, 255);
        }

        .gray-text {
            color: #000000;
            outline: 1px solid #000000;
        }

        .json-data {
            font-family: Arial, sans-serif;
            color: rgb(255, 255, 255);
            text-shadow: -1px -1px 0 black, 1px -1px 0 black, -1px 1px 0 black, 1px 1px 0 black;
        }

        .json-data span {
            color: black;
        }

        @keyframes scrollText {
            0% {
                transform: translateX(100%);
            }
            100% {
                transform: translateX(-100%);
            }
        }

        .cmd-text:hover {
            animation-play-state: paused;
        }

        video {
            position: fixed;
            top: 0;
            left: 0;
            z-index: -1;
            filter: blur(10px);
        }

        /* Hide the audio controls */
        audio {
            display: none;
        }
    </style>
</head>
<body>
    <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animated Text</title>
    <style>
        @keyframes lightning {
            0% { color: rgb(255, 0, 0); }
            50% { color: rgb(0, 0, 0); }
            100% { color: white; }
        }

        .animated-text {
            animation: lightning 1s linear infinite;
        }
    </style>
</head>
<body>
    <h3 class="animated-text">Hmd Passed From Here</h3>
</body>
</html>
    <p id="ip-address">
        <span style="color: rgb(255, 255, 255);">Your IP Address: </span>
        <span id="ip-address-value" style="color: rgb(255, 255, 255); font-size: 17px;">Loading...</span>
    </p>

    <h3 style="color: rgb(255, 255, 255); animation: flashing 1s infinite;">Your IP Info :</h3>
    <pre id="ip-info" class="json-data">Fetching...</pre>
    <div class="cmd-text-container" style="position: relative; top: -15px;">
        <div class="cmd-text" style="font-size: 17px; text-stroke: 3px black; color: black;"> You got hacked by Hmd</div>
    </div>

    <!-- Hidden audio element with autoplay -->
    <audio autoplay loop style="display: none;">
        <source src="" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>

<viedo style="width: 100vw; height: 100vh;" controls autoplay loop muted>
    <source src="">
    Your browser does not support the video element.
</video>


    <script>
        // JavaScript code to fetch and display the user's IP address and information
        function fetchIPAndInfo() {
            fetch('https://api.ipify.org/?format=json')
                .then(response => response.json())
                .then(data => {
                    document.getElementById('ip-address-value').textContent = data.ip;
                    return data.ip;
                })
                .then(ip => fetch(`https://ipinfo.io/${ip}/json`))
                .then(response => response.json())
                .then(ipInfoData => {
                    document.getElementById('ip-info').textContent = JSON.stringify(ipInfoData, null, 2);
                })
                .catch(error => {
                    console.error('Error:', error);
                    document.getElementById('ip-address-value').textContent = 'Unable to fetch IP address.';
                    document.getElementById('ip-info').textContent = 'Unable to fetch IP information.';
                });
        }

        // Fetch IP address and information initially
        fetchIPAndInfo();
    </script>
</body>
</html>
