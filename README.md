# CSS_about_me
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Sawsan Omair - Portfolio</title>
  <link rel="stylesheet" href="styles.css">
  <style>
    body {
      font-family: 'Arial', sans-serif;
      margin: 0;
      padding: 0;
      background: #f4f4f9;
      color: #333;
    }

    .container {
      width: 90%;
      margin: 0 auto;
      max-width: 1200px;
    }

    header {
      background: linear-gradient(to right, #ff7e5f, #feb47b);
      color: white;
      padding: 50px 0;
      text-align: center;
    }

    header h1 {
      margin: 0;
      font-size: 3em;
      font-weight: bold;
      letter-spacing: 1px;
    }

    header p {
      font-size: 1.2em;
      margin-top: 10px;
    }

    section {
      padding: 60px 0;
    }

    section h2 {
      font-size: 2em;
      margin-bottom: 20px;
      text-align: center;
      color: #333;
    }

    .about p {
      font-size: 1.1em;
      line-height: 1.8;
      color: #555;
    }

    .skills .skill {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 20px;
    }

    .skills .progress-bar {
      width: 70%;
      height: 8px;
      background: #ddd;
      border-radius: 4px;
      position: relative;
    }

    .skills .progress-bar.html {
      background: linear-gradient(90deg, #ff7e5f 70%, #ddd 70%);
    }

    .skills .progress-bar.css {
      background: linear-gradient(90deg, #feb47b 60%, #ddd 60%);
    }

    .skills .progress-bar.js {
      background: linear-gradient(90deg, #56ccf2 80%, #ddd 80%);
    }

    .projects .project {
      background: white;
      padding: 20px;
      margin-bottom: 20px;
      border-radius: 8px;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s;
    }

    .projects .project:hover {
      transform: translateY(-10px);
    }

    .projects h3 {
      margin-top: 0;
      color: #333;
      font-size: 1.4em;
    }

    .contact form {
      display: grid;
      gap: 20px;
      max-width: 600px;
      margin: 0 auto;
    }

    .contact input,
    .contact textarea {
      padding: 12px;
      border: 1px solid #ddd;
      border-radius: 4px;
      font-size: 1em;
    }

    .contact button {
      padding: 14px;
      background-color: #ff7e5f;
      color: white;
      font-size: 1.2em;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    .contact button:hover {
      background-color: #feb47b;
    }

    footer {
      background-color: #333;
      color: white;
      padding: 20px 0;
      text-align: center;
    }

    footer a {
      color: #feb47b;
      text-decoration: none;
    }

    footer a:hover {
      text-decoration: underline;
    }

    /* Responsive Styles */
    @media (max-width: 768px) {
      header h1 {
        font-size: 2em;
      }

      .skills .skill {
        flex-direction: column;
        align-items: flex-start;
      }

      .contact form {
        width: 100%;
        padding: 0 20px;
      }
    }

  </style>
</head>
<body>
 
  <header>
    <div class="container">
      <h1>Sawsan Omair</h1>
      <p>Front-End Developer </p>
    </div>
  </header>

  
  <section class="about">
    <div class="container">
      <h2>About Me</h2>
      <p>I am a passionate web developer with experience in HTML, CSS, and JavaScript. I love building user-friendly and responsive websites with great attention to detail and design aesthetics.</p>
      </p>
    </div>
  </section>

  
  <section class="skills">
    <div class="container">
      <h2>My Skills</h2>
      <div class="skill">
        <p>HTML</p>
        <div class="progress-bar html"></div>
      </div>
      <div class="skill">
        <p>CSS</p>
        <div class="progress-bar css"></div>
      </div>
      <div class="skill">
        <p>JavaScript</p>
        <div class="progress-bar js"></div>
      </div>
    </div>
  </section>

  
  <section class="projects">
    <div class="container">
      <h2>My Projects</h2>
      <div class="project">
        <h3>Project 1: Portfolio Website</h3>
        <p>Built a personal portfolio website to showcase my web development skills using HTML, CSS, and JavaScript.</p>
      </div>
      <div class="project">
        <h3>Project 2: Weather App</h3>
        <p>A web application that allows users to get real-time weather data using the OpenWeather API and JavaScript.</p>
      </div>
    </div>
  </section>

  
  <section class="contact">
    <div class="container">
      <h2>Contact Me</h2>
      <form>
        <label for="name">Name:</label>
        <input type="text" id="name" required>
        
        <label for="email">Email:</label>
        <input type="email" id="email" required>

        <label for="message">Message:</label>
        <textarea id="message" required></textarea>

        <button type="submit">Send Message</button>
      </form>
    </div>
  </section>

 
  <footer>
    <div class="container">
      <p>Find me on <a href="#">GitHub</a> </p>
    </div>
  </footer>

  <script src="scripts.js"></script>
</body>
</html>
