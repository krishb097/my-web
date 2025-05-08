<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Thank You</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: white;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
    }
    .thank-you-box {
      background-color: rgb(10, 232, 248);
      padding: 30px 40px;
      border-radius: 10px;
      box-shadow: 0 0 15px rgb(10, 0, 0);
      text-align: center;
      transition: all 0.3s ease;
    }
    .thank-you-box:hover {
      background-color: transparent;
      border: 1px solid black;
      transform: scale(1.1);
    }
    .thank-you-box h1 {
      color: lightseagreen;
      font-size: 28px;
    }
    .thank-you-box p {
      margin-top: 10px;
      font-size: 16px;
      color: #110707;
    }
  </style>
</head>
<body>
  <div class="thank-you-box">
    <h1>Thank you for your feedback.</h1>
    <p>We truly appreciate your input !!</p>
  </div>
</body>
</html>
