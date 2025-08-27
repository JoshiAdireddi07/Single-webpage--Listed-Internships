# Single-webpage--Listed-Internships
a single internship webpage where instead of just showing the title + duration/location/start date, each internship card also includes a short description in context following with the respective link.

    <!DOCTYPE html>
    <html lang="en">
     <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>VaultofCodes - Internship Programs</title>
     <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      min-height: 100vh;
      padding: 40px 20px;
      color: #333;
      background: linear-gradient(270deg, #DAD7CD, #A3B18A, #588157, #3A5A40, #344E41);
      background-size: 800% 800%;
      animation: gradientShift 25s ease infinite;
    }

    @keyframes gradientShift {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    .container { max-width: 1200px; margin: 0 auto; }

    .header { text-align: center; margin-bottom: 50px; }

    .logo {
      color: #DAD7CD;
      font-size: 2rem;
      font-weight: 300;
      letter-spacing: 2px;
      margin-bottom: 20px;
      text-shadow: 2px 2px 6px rgba(0,0,0,0.4);
    }

    .title {
      font-size: 3.5rem;
      font-weight: 700;
      margin-bottom: 20px;
      background: linear-gradient(90deg, #DAD7CD, #A3B18A, #588157, #3A5A40, #344E41);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-size: 300% 300%;
      animation: gradientShift 10s ease infinite;
    }

    .internships-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
      gap: 30px;
    }

    .internship-card {
      background: rgba(255, 255, 255, 0.95);
      border-radius: 20px;
      padding: 30px;
      box-shadow: 0 20px 40px rgba(0,0,0,0.15);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      position: relative;
    }

    .internship-card:hover {
      transform: translateY(-10px) scale(1.02);
      box-shadow: 0 30px 60px rgba(0,0,0,0.2);
    }

    .tech-icon {
      width: 50px; height: 50px;
      border-radius: 50%;
      display: flex; align-items: center; justify-content: center;
      font-size: 1.5rem;
      margin: 0 auto 15px;
      color: white; font-weight: bold;
    }

    .web-dev .tech-icon { background: linear-gradient(135deg, #588157, #3A5A40); }
    .app-dev .tech-icon { background: linear-gradient(135deg, #A3B18A, #588157); }
    .python-dev .tech-icon { background: linear-gradient(135deg, #344E41, #588157); }

    .card-title {
      font-size: 1.4rem;
      font-weight: 700;
      color: #2c3e50;
      margin-bottom: 15px;
      text-align: center;
    }

    .card-desc {
      font-size: 1rem;
      color: #555;
      line-height: 1.5;
      margin-bottom: 20px;
      text-align: center;
    }

    .card-details {
      list-style: none;
      margin-bottom: 20px;
      padding: 0;
    }

    .card-details li {
      display: flex; justify-content: space-between;
      padding: 8px 0;
      border-bottom: 1px solid rgba(0,0,0,0.1);
      font-size: 0.95rem;
    }

    .card-details li:last-child { border-bottom: none; }

    .detail-label { font-weight: 600; color: #2c3e50; }
    .detail-value { color: #666; }

    .view-details-btn {
      display: block;
      width: 100%;
      padding: 12px;
      text-align: center;
      background: linear-gradient(135deg, #3A5A40, #588157);
      color: white;
      font-weight: bold;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      text-decoration: none;
      transition: background 0.3s ease;
    }

    .view-details-btn:hover {
      background: linear-gradient(135deg, #588157, #3A5A40);
    }

    @media (max-width: 768px) {
      .title { font-size: 2.5rem; }
    }
    </style>
      </head>
     <body>
     <div class="container">
      <div class="header">
       <div class="logo">VaultofCodes</div>
      <h1 class="title">Internship Programs</h1>
    </div>

    <div class="internships-grid">
      <!-- Web Dev Internship -->
      <div class="internship-card web-dev">
        <div class="tech-icon">🌐</div>
        <h2 class="card-title">Web Development Internship</h2>
        <p class="card-desc">
          Build modern, responsive websites using HTML, CSS, JavaScript, and frameworks.
          Learn real-world skills by working on hands-on projects.
        </p>
        <ul class="card-details">
          <li><span class="detail-label">Duration</span><span class="detail-value">1-2 months</span></li>
          <li><span class="detail-label">Location</span><span class="detail-value">Virtual</span></li>
          <li><span class="detail-label">Stipend</span><span class="detail-value">Unpaid</span></li>
          <li><span class="detail-label">Start Date</span><span class="detail-value">05/11/2023</span></li>
        </ul>
        <a href="https://www.codecademy.com/learn/paths/web-development" target="_blank" class="view-details-btn">View Details</a>
      </div>

      <!-- App Dev Internship -->
      <div class="internship-card app-dev">
        <div class="tech-icon">📱</div>
        <h2 class="card-title">App Development Internship</h2>
        <p class="card-desc">
          Dive into Android app development with Java/Kotlin. Create functional mobile apps,
          improve UI/UX, and publish prototypes.
        </p>
        <ul class="card-details">
          <li><span class="detail-label">Duration</span><span class="detail-value">1-2 months</span></li>
          <li><span class="detail-label">Location</span><span class="detail-value">Virtual</span></li>
          <li><span class="detail-label">Stipend</span><span class="detail-value">Unpaid</span></li>
          <li><span class="detail-label">Start Date</span><span class="detail-value">05/11/2023</span></li>
        </ul>
        <a href="https://developer.android.com/courses" target="_blank" class="view-details-btn">View Details</a>
      </div>

      <!-- Python Internship -->
      <div class="internship-card python-dev">
        <div class="tech-icon">🐍</div>
        <h2 class="card-title">Python Programming Internship</h2>
        <p class="card-desc">
          Master Python fundamentals and apply them in projects involving automation, 
          data handling, and problem-solving tasks.
        </p>
        <ul class="card-details">
          <li><span class="detail-label">Duration</span><span class="detail-value">1-2 months</span></li>
          <li><span class="detail-label">Location</span><span class="detail-value">Virtual</span></li>
          <li><span class="detail-label">Stipend</span><span class="detail-value">Unpaid</span></li>
          <li><span class="detail-label">Start Date</span><span class="detail-value">05/11/2023</span></li>
        </ul>
        <a href="https://www.python.org/about/gettingstarted/" target="_blank" class="view-details-btn">View Details</a>
      </div>
    </div>
     </div>
     </body>
    </html>
