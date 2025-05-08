<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About</title>
    <style>
        body {
            background-image: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1740&q=80');
      }
       div a {
            display: inline-block;
            background-color: white;
            color: black;
            padding: 10px 20px;
            text-decoration: none;
            border-radius: 4px;
            font-weight: bold;
            transition: all 0.3s ease;         
            }

        div a:hover {
            background-color: transparent;
            color: black;
            border: 1px solid black;
            text-decoration: underline;
            transform: scale(1.1);
        }

        nav {
            background-color: #333;
            color: white;
            padding: 10px;
            text-align: center;
        }

        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
        }

        nav a:hover {
            text-decoration: underline;
        }
        .logout a {
      text-align: center;
      margin: 10px;
      color: white;
      background-color: #333;
      text-decoration: none;
      transition: all 0.3s ease;
    }
    .logout a:hover {
      background-color: transparent;
      color: white;
      border: 1px solid white;
      text-decoration: underline;
      transform: scale(1.1);
    }
    section {
      margin: 15px;
      padding-top: 10px;
      padding-bottom: 10px;
      background-color: transparent;
      border: none;
      border-radius: 5px;
      box-shadow: 0 0 20px rgb(8, 0, 0);
    }
    </style>
</head>
<body>
    <nav>
        <a href="home.html">Home</a>
        <a href="about.html">About</a>
        <a href="contact.html">Contact</a>
        <a href="feedback.html">Feedback</a>
        <div class="logout">
            <a href="log.html">Logout</a>
        </div>
    </nav>

    <section>
        <div style="max-width: 900px; margin: 20px;">
        <b>
            <u><h2 style="color: #080000">About Us</h2></u>
            <p style="font-size: 1.1em; color: #080000;">
                Welcome to our website! We are a team of passionate developers and designers dedicated to creating the best virtual meeting platforms.
            </p>
            <p style="font-size: 1.1em; color: #080000;">
                These are our company's values.
            </p>
            <h3 style="margin-top: 30px; color: #080000;">Our Values</h3>
            <ul style="line-height: 1.8; color: #080000;">
                <li>✔️ Best Quality of Video and Audio.</li>
                <li>✔️ Transparent communication</li>
                <li>✔️ Longtime Video Chats.</li>
                <li>✔️ Comfortable for studies and meetings.</li>
            </ul>
            <p style="font-size: 1.1em; color: #080000;">
                For more information, contact us.<br>
            </p>
            </b>
            <div class="div">
                <a href="contact.html">Contact</a>
                <p style="font-size: 1.1em; color: #080000;"><b>
                    Go to the Home Section for more information about user operations.
                </p></div>
                <a href="home.html">Home</a>
            </div>
        </div>
    </section>
</body>
</html>
