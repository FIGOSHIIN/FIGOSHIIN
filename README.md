<!DOCTYPE html>
<html>
    <head>
<meta charset="UTF-8">
<link rel="icon" href="./favicon.ico" />
<meta name="theme-color" content="#43AFFC" />
<link rel="manifest" href="./manifest.json" />
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Weather app</title>
<link rel="stylesheet" href="./style.css">
<!-- icon's link -->
<link href='https://unpkg.com/boxicons@2.0.9/css/boxicons.min.css' rel='stylesheet'>
    </head>
    <body>
        <script type="module">
            // Import the functions you need from the SDKs you need
            import { initializeApp } from "https://www.gstatic.com/firebasejs/9.1.0/firebase-app.js";
            import { getAnalytics } from "https://www.gstatic.com/firebasejs/9.1.0/firebase-analytics.js";
            // TODO: Add SDKs for Firebase products that you want to use
            // https://firebase.google.com/docs/web/setup#available-libraries
          
            // Your web app's Firebase configuration
            // For Firebase JS SDK v7.20.0 and later, measurementId is optional
            const firebaseConfig = {
              apiKey: "AIzaSyDiGch33zc9lVAHgyQcdOJNnhZ3s_at6Ao",
              authDomain: "myweath-app.firebaseapp.com",
              projectId: "myweath-app",
              storageBucket: "myweath-app.appspot.com",
              messagingSenderId: "60479205173",
              appId: "1:60479205173:web:e50b0e90bc6bbd7073a67c",
              measurementId: "G-CHX6B89F7E"
            };
          
            // Initialize Firebase
            const app = initializeApp(firebaseConfig);
            const analytics = getAnalytics(app);
          </script>

          
<div class="wrraper">
    <header><i class="bx bx-left-arrow-alt"></i>Weather App</header>
    <section class="input-part">
        <p class="info-txt"></p>
        <input type="text" placeholder="Enter city name" spellcheck="False" required>
        <div class="seperator"></div>
        <button>Get Device Location</button>
    </section>
    <section class="weather-part">
        <img id="icon" alt="weather icon">
       <div class="temp">
           <span class="numb">_</span>
           <span class="deg">°</span>C
       </div>
<div class="weather">_ _</div>
<div class="location">
    <i class="bx bx-map"></i>
    <span>_, _</span>
</div>
    <div class="bottom-details">
     <div class="column feels">
         <i class="bx bxs-thermometer"></i> 
         <div class="details">
            <div class="temp">
                <span class="numb-2">_</span>
                <span class="deg">°</span>C
            </div>
        <P>Feels like</P>
</div>
</div>
<div class="column humidity">
    <i class="bx bxs-droplet-half"></i> 
    <div class="details">
    <span>_</span>
   <P>Humidity</P>

</div>
</div>
</div>
    </section>
</div>
<script src="script.js"></script>
    </body>
</html>
