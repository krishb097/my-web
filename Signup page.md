<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Signup - VMEET</title>
  <style>
    body {
      background-image: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1740&q=80');
      font-family: Arial, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }

    .signup-container {
      background-color: transparent;
      padding: 50px;
      border-radius: 8px;
      box-shadow: 0 0 10px rgb(7, 1, 1);
      width: 100%;
      max-width: 500px;
    }

    h2 {
      text-align: center;
      margin-bottom: 20px;
      color: #333;
    }

    input {
      background-color: rgb(120, 212, 243);
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      border-radius: 5px;
      border: 1px solid black;
      transition: all 0.3s ease;
    }

    input:hover {
      background-color: transparent;
      transform: scale(1.1);
    }

    button {
      width: 100%;
      margin-left: 10px;
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
      border: 1px solid black;
      border-radius: 4px;
      transform: scale(1.1);
    }

    .signup-container a {
      display: inline-block;
      background-color: blue;
      color: white;
      padding: 10px 20px;
      text-decoration: none;
      border-radius: 4px;
      font-weight: bold;
      transition: all 0.3s ease;
    }

    .signup-container a:hover {
      text-decoration: underline;
      transform: scale(1.1); 
    }

    .login-link {
      text-align: center;
      margin-top: 15px;
      margin-left: 5px;
    }

    .login-link a {
      text-decoration: none;
      background-color: white;
      color: black;
      font-weight: bold;
    }

    .login-link a:hover {
      background-color: transparent;
      text-decoration: underline;
      color: black;
      border: 1px solid black;
    }
  </style>
</head>
<body>

  <div class="signup-container">
    <h2>Signup for VMEET</h2>
    <form onsubmit="redirectToLogin(); return false;">
        <input type="text" name="fullname" placeholder="Full Name" required />
        <input type="email" name="email" placeholder="Email" required />
        <input type="text" name="username" placeholder="Username" required />
        <input type="password" name="password" placeholder="Password" required />
        <button type="submit">Create Account</button>
    </form>

    <div class="login-link">
      <b>
      Already have an account? <a href="log.html">Login here</a>
      </b>
    </div>
  </div>

  <script>
    function redirectToLogin() {
      // Simulate signup logic here (optional)
      alert("Account created successfully!");
      window.location.href = "log.html"; // Redirect to login page
    }
  </script> 

</body>
</html>
