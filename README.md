# Dinero-tools-
TECH SUPPORT
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dinero Tools</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg-color: #f8f9fa;
      --text-color: #333;
      --header-bg: #343a40;
      --header-text: #fff;
      --highlight: #ffc107;
    }

    [data-theme="dark"] {
      --bg-color: #1e1e1e;
      --text-color: #eaeaea;
      --header-bg: #121212;
      --header-text: #f1f1f1;
      --highlight: #ffca28;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Roboto', sans-serif;
    }
    body {
      background-color: var(--bg-color);
      color: var(--text-color);
      line-height: 1.6;
      transition: background-color 0.3s, color 0.3s;
    }
    header {
      background-color: var(--header-bg);
      color: var(--header-text);
      padding: 1rem 2rem;
      text-align: center;
    }
    nav {
      margin-top: 10px;
    }
    nav a {
      color: var(--highlight);
      margin: 0 15px;
      text-decoration: none;
    }
    .theme-toggle {
      margin-top: 10px;
      background: var(--highlight);
      border: none;
      padding: 0.5rem 1rem;
      cursor: pointer;
      color: #000;
      border-radius: 5px;
    }
    .hero {
      text-align: center;
      padding: 4rem 2rem;
      background: linear-gradient(to right, var(--bg-color), #e9ecef);
    }
    .hero h1 {
      font-size: 3rem;
      margin-bottom: 1rem;
    }
    .hero p {
      font-size: 1.25rem;
      color: var(--text-color);
    }
    .features {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 2rem;
      padding: 3rem 2rem;
    }
    .feature {
      background-color: #fff;
      padding: 2rem;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
      text-align: center;
    }
    [data-theme="dark"] .feature {
      background-color: #2c2c2c;
    }
    .feature h3 {
      margin-bottom: 1rem;
      color: var(--header-bg);
    }
    footer {
      background-color: var(--header-bg);
      color: #ccc;
      text-align: center;
      padding: 1.5rem 2rem;
      margin-top: 2rem;
    }
    .payment, .whatsapp {
      text-align: center;
      margin: 2rem 0;
    }
    .whatsapp a {
      color: green;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <header>
    <h1>Dinero Tools</h1>
    <nav>
      <a href="#">Home</a>
      <a href="#tools">Tools</a>
      <a href="#contact">Contact</a>
    </nav>
    <button class="theme-toggle" onclick="toggleTheme()">Toggle Theme</button>
  </header>

  <section class="hero">
    <h1>Welcome to Dinero Tools</h1>
    <p>Your all-in-one destination for powerful developer tools, APIs, and tech resources.</p>
  </section>

  <section class="features" id="tools">
    <div class="feature">
      <h3>Code Utilities</h3>
      <p>Access a suite of tools to help you write, debug, and deploy code efficiently.</p>
    </div>
    <div class="feature">
      <h3>API Integrations</h3>
      <p>Explore ready-to-use API integrations for your applications and services.</p>
    </div>
    <div class="feature">
      <h3>Support & Docs</h3>
      <p>Comprehensive documentation and guides to get you started in minutes.</p>
    </div>
  </section>

  <section class="payment">
    <h2>💳 Make a Payment</h2>
    <p>We accept secure payments via Flutterwave and PayPal.</p>
    <p><a href="#">Pay Now</a> (Coming soon)</p>
  </section>

  <section class="whatsapp">
    <h2>📞 Chat with Us</h2>
    <p>Need help or have questions? <a href="https://wa.me/2349012345678" target="_blank">Chat on WhatsApp</a></p>
  </section>

  <footer id="contact">
    <p>&copy; 2025 Dinero Tools. All rights reserved.</p>
  </footer>

  <script>
    function toggleTheme() {
      const body = document.body;
      const theme = body.getAttribute('data-theme');
      body.setAttribute('data-theme', theme === 'dark' ? 'light' : 'dark');
    }

    // Default to light theme
    document.body.setAttribute('data-theme', 'light');
  </script>
</body>
</html>
