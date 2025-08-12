<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>{{ page.title }} | {{ site.title }}</title>
  <style>
    body {
      margin: 0;
      font-family: 'Helvetica Neue', Arial, sans-serif;
      background-color: #222222;
      color: #f5f5f5;
      line-height: 1.6;
    }
    a {
      color: #ffcc66;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
    header, footer {
      text-align: center;
      padding: 1rem;
    }
    .intro {
      text-align: center;
      padding: 2rem;
    }
    .intro-image {
      max-width: 100%;
      height: auto;
      border-radius: 8px;
      margin-bottom: 1rem;
    }
    h1 {
      font-size: 2rem;
      margin-bottom: 0.5rem;
    }
    .tagline {
      font-size: 1.2rem;
      color: #ccc;
    }
    .about {
      max-width: 700px;
      margin: 0 auto;
      padding: 2rem;
    }
    .emoji {
    font-size: 1.2rem;   /* Change emoji size only */
    vertical-align: middle; /* Keeps it aligned with text */
    }
    .highlights {
    display: flex;
    justify-content: center;
    align-items: stretch;
    gap: 20px;
    padding: 20px;
    flex-wrap: wrap; /* Makes it stack on small screens */
    }
    .highlight-box {
      flex: 1 1 250px; /* Min width of box */
      max-width: 300px;
      background: #f8f9fa;
      border: 1px solid #ddd;
      border-radius: 10px;
      padding: 15px;
      text-align: center;
      box-shadow: 0px 2px 5px rgba(0,0,0,0.1);
      transition: transform 0.2s ease, box-shadow 0.2s ease;
    }
    .highlight-box:hover {
      transform: translateY(-3px);
      box-shadow: 0px 4px 10px rgba(0,0,0,0.15);
    }
    .highlight-box h2 {
      font-size: 1.2rem;
      margin-bottom: 10px;
    }
    .highlight-box a {
      color: #007acc;
      text-decoration: none;
    }
    .highlight-box a:hover {
      text-decoration: underline;

  </style>

  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twemoji/14.0.2/twemoji.min.css">
  <script src="https://twemoji.maxcdn.com/v/latest/twemoji.min.js" crossorigin="anonymous"></script>
  <script>
    document.addEventListener("DOMContentLoaded", function() {
      twemoji.parse(document.body, { folder: 'svg', ext: '.svg' });
    });
  </script>
</head>
<body>
  <header>
    <nav>
      <a href="/">Home</a> |
      <a href="/about/">About</a> |
      <a href="/team/">Team</a> |
      <a href="/transients/">Transients!!!</a> |
      <a href="/news/">News</a> |
      <a href="/publications/">Publications</a>
    </nav>
  </header>

  <main>
    {{ content }}
  </main>

  <footer>
    &copy; {{ site.time | date: "%Y" }} {{ site.title }} — All rights reserved.
  </footer>
</body>
</html>
