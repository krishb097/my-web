<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Login - VMEET</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      height: 100%;
      font-family: Arial, sans-serif;
    }

    body {
      background-image: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1740&q=80');
      background-size: cover;
      background-position: center;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      align-items: center;
      padding-bottom: 60px;
    }

    nav {
      background-color: #333;
      color: white;
      padding: 10px;
      text-align: center;
      width: 100%;
    }

    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
    }

    nav a:hover {
      text-decoration: underline;
    }

    form {
      background: transparent;
      padding: 30px;
      border-radius: 8px;
      box-shadow: 0 0 20px rgb(8, 0, 0);
      max-width: 400px;
      width: 100%;
      margin-top: 40px;
    }

    form h2 {
      margin-bottom: 20px;
      text-align: center;
    }

    input[type="text"],
    input[type="password"] {
      background-color: rgb(120, 212, 243);
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      border-radius: 5px;
      border: 1px solid black;
      transition: all 0.3s ease;
    }
    input[type="password"]:hover {
      background-color: transparent;
      transform: scale(1.1);
    }
    input[type="text"]:hover {
      background-color: transparent;
      transform: scale(1.1);
    }

    button {
      width: 100%;
      padding: 10px;
      background-color: rgb(33, 218, 33);
      color: white;
      border: none;
      font-size: 16px;
      cursor: pointer;
      border-radius: 5px;
      margin-top: 20px;
      transition: all 0.3s ease;
    }

    button:hover {
      background-color: transparent;
      color: black;
      border-radius: 4px;
      border: 1px solid black;
      transform: scale(1.1);
    }

    .signup-link {
      text-align: center;
      margin-top: 20px;
    }

    .signup-link a {
      display: inline-block;
      background-color: white;
      color: black;
      margin-top: 10px;
      padding: 10px 20px;
      text-decoration: none;
      border-radius: 4px;
      font-weight: bold;
      transition: all 0.3s ease;
    }

    .signup-link a:hover {
      background-color: transparent;
      color: black;
      border: 1px solid black;
      text-decoration: underline;
      transform: scale(1.1);
    }

    footer {
      background-color: transparent;
      border: 2px solid black;
      box-shadow: 0, 0, 20px rgb(10, 0, 0);
      text-align: center;
      padding: 10px;
      position: fixed;
      width: 100%;
      bottom: 0;
      left: 0;
    }
  </style>
</head>
<body>

  <nav>
    <a href="home.html">Home</a>
    <a href="about.html">About</a>
    <a href="contact.html">Contact</a>
    <a href="feedback.html">Feedback</a>
  </nav>

  <form onsubmit="return handleLogin(event)">
    <h2>Login to VMEET</h2>

    <input type="text" id="username" placeholder="Enter your username" required />

    <input type="password" id="password" placeholder="Enter your password" required />

    <button type="submit">Login</button>

    <div class="signup-link">
      <p><b>You don't have an account?</b></p>
      <a href="signup.html">Sign up</a>
    </div>
  </form>

  <footer>
    <b>&copy; 2025 | VMEET Software</b>
  </footer>
  <script>
    window.alert("Welcome To The VMEET Software.")
  </script>
  <script>
    function handleLogin(event) {
      event.preventDefault();
      const username = document.getElementById('username').value.trim();
      const password = document.getElementById('password').value.trim();

      if (username && password) {
        localStorage.setItem("loginSuccess", "true");
        window.location.href = "home.html";
      } else {
        alert("Please enter a valid username and password.");
      }
      return false;
    }
  </script>

</body>
</html>
