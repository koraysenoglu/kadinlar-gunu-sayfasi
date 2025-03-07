<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eda ♡ Koray</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #ffe6f2;
            padding: 50px;
        }
        h1 {
            font-size: 36px;
            color: #d63384;
        }
        button {
            background-color: #ff4d79;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 18px;
            margin: 10px;
            cursor: pointer;
            border-radius: 10px;
        }
        button:hover {
            background-color: #cc004d;
        }
        p {
            font-size: 20px;
            margin-top: 20px;
        }
        #message {
            font-size: 24px;
            font-weight: bold;
        }
        #photo {
            max-width: 20%;
            height: auto;
            margin-top: 20px;
            display: none;
            margin-left: auto;
            margin-right: auto;
        }
        .gif-container {
            margin-top: 30px;
        }
        #gif {
            max-width: 80%;
            display: block;
            margin: 20px auto;
        }
    </style>
</head>
<body>
    <h1>Eda'ya sevgilerimle ❤️</h1>
    <button onclick="toggleMessage()">Eeee şey...</button>
    <button onclick="togglePhoto()">Bu butona tıkladıktan sonra hayatımda daha güzel bir görüntü göremeyeceğimi kabul ediyorum!</button>
    <p id="message"></p>
    <img id="photo" src="" alt="Biz">
    <p>Kadınlar günün kutlu olsun bir tanem. Yanında olamadığım için en efektif yolun bu olacağını düşündüm.</p>
    
    <div class="gif-container">
        <img src="gif.gif" alt="Kutlama Gif" id="gif">
    </div>
    
    <script>
        function toggleMessage() {
            let message = document.getElementById("message");
            if (message.innerText === "") {
                message.innerText = "Bugün çok güzel olduğunu söylemiş miydim?";
            } else {
                message.innerText = "";
            }
        }
        
        function togglePhoto() {
            let photo = document.getElementById("photo");
            if (photo.style.display === "none" || photo.style.display === "") {
                photo.src = "biz.jpg";
                photo.style.display = "block";
            } else {
                photo.style.display = "none";
            }
        }
    </script>
</body>
</html>
