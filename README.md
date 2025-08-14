<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Birthday Card</title>
  <link href="https://fonts.googleapis.com/css2?family=Mali&family=Jua&display=swap" rel="stylesheet">
  <style>
    body {
      background: #fef0f5;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
    }

    .card-container {
      width: 600px;
      perspective: 2000px;
    }

    .card {
      width: 100%;
      position: relative;
    }

    .cover {
      width: 100%;
      height: 550px;
      background: url('https://ibb.co/5Xvpphb1') center/cover no-repeat;
      position: absolute;
      left: 0;
      top: 0;
      z-index: 2;
      transform-origin: left;
      transform: rotateY(0deg);
      transition: transform 1.2s ease-in-out;
      border-radius: 10px;
      border: 5px solid white;
      display: flex;
      justify-content: center;
      align-items: center;
      cursor: pointer;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
      box-sizing: border-box;
    }

    .card.open .cover {
      transform: rotateY(-180deg);
    }

    .inside {
      width: 100%;
      height: 550px;
      background: white;
      position: relative;
      z-index: 1;
      border-radius: 10px;
      padding: 20px;
      box-sizing: border-box;
      text-align: left;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
      overflow-y: auto;
      font-family: 'Mali', sans-serif;
      font-size: 20px;
      color: #ebafab;
    }

    .inside .heart {
      font-size: 40px;
      color: #ffdbd9;
      animation: beat 1s infinite;
      margin-bottom: 15px;
      text-align: center;
    }

    .inside h1 {
      font-family: 'Jua', sans-serif;
      font-size: 36px;
      color: #ffdbd9;
      margin-bottom: 20px;
      text-align: center;
      font-weight: bold;
    }

    .inside p {
      line-height: 1.6;
      margin-bottom: 10px;
      white-space: pre-line;
    }

    @keyframes beat {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.2); }
    }
  </style>
</head>
<body>
  <div class="card-container">
    <div class="card" id="card" onclick="openCard()">
      <div class="cover"></div>
      <div class="inside">
        <h1> HAPPY 15TH BDAY !! </h1>
        <div class="heart">♥</div>
        <p>

HAPPY BIRTHDAY TOLLLL, MISS YOU SMM!
Hwehwehw lowk andami kong gustong sabihin hahah but first, I just wanna say how much I appreciate you 
so saur much. You’re one of the most AMAZING, MABAIT, and UNDERSTANDING people I know hihihi. You have 
no idea how grateful I am that I met and got to know a person like you.

We’ve only known each other for a few years, pero highkey it feels like ang tagal na nating magkaibigan, 
kahit minsan bitin pa nga ang pagsasama natin hwahahaha. Miss ko narin mga , tawanan natin sa gilid kahit
walang sense minsan hahaha, chikahan and pag palaging magkatabi tayo. Those moments would made my whole day 
during Grade 8 frfr. And btw ang dami ng nakakamiss sayo sa USL HAHAHA

I’m also super duper thankful na you were always there for me when I was at my lowest, lalo na noong Grade 8. 
You listened to me kahit you were going through your own struggles too huhu and that means so much to me. You 
hab no idea how much your presence helped me get through those times hihi. 

And I want you to know that I’m always here for you, no matter what hehe. I hope your day is filled with nothing 
but love, happiness, and blessings because you truly deserve it. Sana maglast pa tayo for many more years to come, 
and I excited ako for next gala natin hihi.


        </p>
      </div>
    </div>
  </div>

  <script>
    function openCard() {
      document.getElementById("card").classList.toggle("open");
    }
  </script>
</body>
</html>
