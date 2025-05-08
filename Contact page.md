<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Contact Us - VMEET</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-image: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1740&q=80');
    }

    .contact-section {
      max-width: 800px;
      margin: 50px auto;
      padding: 30px;
      background-color: transparent;
      border-radius: 8px;
      box-shadow: 0 0 10px rgb(8, 0, 0);
      width: 100%;
    }

    .contact-section h2 {
      text-align: center;
      margin-bottom: 20px;
    }

    .contact-info {
      margin-bottom: 30px;
      text-align: center;
    }

    .contact-info p {
      margin: 8px 0;
      font-size: 16px;
    }

    form {
      display: flex;
      flex-direction: column;
    }

    input, textarea {
      padding-left: 10px;
      padding-right: 10px;
      padding: 10px;
      margin-bottom: 15px;
      background-color: rgb(120, 212, 242);
      border: none;
      border-radius: 4px;
      font-size: 16px;
      width: 100%;
      box-sizing: border-box;
      transition: all 0.3s ease;
    }
    input:hover {
      border: 1px solid black;
      background-color: transparent;
      transform: scale(1.1);
    }
    textarea:hover{
      border: 1px solid black;
      background-color: transparent;
      transform: scale(1.1);
    }

    button {
      padding: 10px;
      background-color: rgb(35, 211, 35);
      color: white;
      border: none;
      border-radius: 4px;
      font-size: 16px;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    button:hover {
      background-color: transparent;
      border: 1px solid black;
      color: black;
      transform: scale(1.1);
    }

    @media (max-width: 600px) {
      .contact-section {
        margin: 20px;
        padding: 20px;
      }
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
  </style>
</head>
<body>
  <nav>
    <a href="home.html">Home</a>
    <a href="about.html">About</a>
    <a href="contact.html">Contact</a>
    <a href="feedback.html">Feedback</a>
  </nav>

  <section class="contact-section">
    <h2><u>Contact Us</u></h2>

    <div class="contact-info">
      <p><strong>Email:</strong> krishnabarot544@gmail.com</p>
      <p><strong>Phone:</strong> +91-7990234132</p>
      <p><strong>Address:</strong> Barot - Vas, Unava, Unjha - Mehsana, Gujarat.</p>
    </div>

    <form action="submit_contact.html" method="post">
      <input type="text" name="name" placeholder="Your Name" required />
      <input type="email" name="email" placeholder="Your Email" required />
      <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>

  </section>
</body>
</html>
