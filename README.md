<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <title>Music Website</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

    <div class="hero">
         <div class="navbar">
             <img src="images/logo.png" class="logo">
             <ul>
                 <li><a href="#">HOME</a></li>
                 <li><a href="#">ABOUT</a></li>
                 <li><a href="#">SPECIFICATION</a></li>
                 <li><a href="#">PRODUCTS</a></li>
                 <li><a href="#">CONTACT</a></li>
             </ul>
          </div>
          <div class="content">
              <div class="left">
                   <h1>THE <br> REAL <br> MUSIC</h1>
              </div>
              <div class="right">
                   <button id="play">Play</button>
              </div>
              <div>
                <button id="pause">Pause</button>
              </div>
          </div>
     </div>

     <audio id="mysong">
         <source src="Om shanti om instrumental.mp3" type="audio/mp3">
     </audio>

     <script>

          var mysong = document.getElementById("mysong");
          var play = document.getElementById("play");
          var pause = document.getElementById("pause")


          play.addEventListener('click',()=>
          {
            mysong.play()
          })   
          pause.addEventListener('click',()=>
          {
            mysong.pause()
          }) 

      </script>


 </body>
 </html>
