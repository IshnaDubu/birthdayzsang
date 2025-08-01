<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy Birthday, Lovey!</title>
  <link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Quicksand:wght@400;600&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Quicksand', sans-serif;
      background-color: #ffe4e9;
      background-image: url('https://www.transparenttextures.com/patterns/pink-dust.png');
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      text-align: center;
    }
    .container {
      background-color: white;
      padding: 2.5rem;
      border-radius: 2rem;
      box-shadow: 0 0 30px rgba(255, 182, 193, 0.4);
      max-width: 800px;
      width: 90%;
      border: 4px solid #fbb6ce;
      position: relative;
    }
    h1 {
      color: #d63384;
      font-family: 'Pacifico', cursive;
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
    }
    .date {
      font-size: 1rem;
      color: #888;
      margin-bottom: 1.5rem;
    }
    .envelope {
      background-color: #ffb6c1;
      padding: 1.5rem;
      border-radius: 1rem;
      margin-top: 1rem;
      cursor: pointer;
      transition: all 0.3s ease;
      color: white;
      font-weight: bold;
    }
    .envelope:hover {
      background-color: #ff80a8;
    }
    .letter {
      white-space: pre-wrap;
      color: #4b1e2f;
      text-align: justify;
      max-height: 600px;
      overflow-y: auto;
      margin-top: 2rem;
      font-size: 1.1rem;
      line-height: 2.2;
      padding: 0 1.5rem;
      display: none;
    }
    .show {
      display: block;
    }
    .decor {
      position: absolute;
      top: -20px;
      right: -20px;
      width: 80px;
    }
    .bottom-image {
      margin-top: 2rem;
      max-width: 100%;
      border-radius: 1rem;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    }
    .confetti {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-image: url('https://png.pngtree.com/png-vector/20220713/ourmid/pngtree-cute-confetti-pink-background-png-image_5895400.png');
      background-size: cover;
      opacity: 0.05;
      z-index: 0;
      border-radius: 2rem;
    }
    audio {
      margin-top: 1.5rem;
      width: 100%;
      max-width: 600px;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="confetti"></div>
    <h1>🎀 Happy Birthday, Lovey! 🎀</h1>
    <div class="date">August 2, 2025</div>
    <img class="decor" src="https://emojicdn.elk.sh/🎂" alt="cake">
    <div id="envelope" class="envelope">💌 Open Envelope</div>
    <div id="letter" class="letter">
Maligayang Kaarawan, Akong Misis!!!

Lovey, sobrang hanga ako at buhay pa tayo sa gantong edad hahaha gago ng buhay eh noh? pero mas nagiging tolerable ang lahat dahil buo pa rin tayo...
    </div>
    <img class="bottom-image" src="https://drive.google.com/uc?export=view&id=1naq55UoJh5QiPFfjrIgMC_TOsZuNNZef" alt="us" />
    <audio controls>
      <source src="https://dl.dropboxusercontent.com/scl/fi/zfhyxt21fqy7qngjmmocd/bg-music.mp3?rlkey=2u0cw2ftdsd3pm1v7m8qbdpgu&dl=0" type="audio/mpeg">
      Your browser does not support the audio element.
    </audio>
  </div>
  <script>
    const envelope = document.getElementById('envelope');
    const letter = document.getElementById('letter');

    envelope.addEventListener('click', () => {
      letter.classList.toggle('show');
      envelope.style.display = 'none';
    });
  </script>

  <button id="playMusicBtn" style="
    margin-top: 20px;
    padding: 1rem 2rem;
    font-size: 1rem;
    background-color: #ff69b4;
    color: white;
    border: none;
    border-radius: 1rem;
    cursor: pointer;
    box-shadow: 0 4px 10px rgba(0,0,0,0.2);
  ">Click to Start the Surprise 🎵</button>

  <script>
    const audio = new Audio('happy-birthday.mp3');
    const button = document.getElementById('playMusicBtn');
    button.addEventListener('click', () => {
      audio.play();
      button.style.display = 'none'; // hide after clicking
    });
  </script>

</body>
</html>
