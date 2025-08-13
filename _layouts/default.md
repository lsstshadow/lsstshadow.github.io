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
      font-size: 4rem;
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
      font-size: 1.2em;   /* Change emoji size only */
      vertical-align: middle; /* Keeps it aligned with text */
    }
    .highlights {
      display: flex;
      justify-content: center;
      align-items: stretch;
      gap: 20px;
      padding: 20px;
      flex-wrap: wrap; /* Responsive stacking on small screens */
    } 
    .highlight-box {
      flex: 1 1 250px;
      max-width: 300px;
      background: #1c1c1c; /* Dark theme */
      color: #f8f8f8;
      border: 1px solid #444;
      border-radius: 10px;
      padding: 15px;
      text-align: center;
      box-shadow: 0px 2px 6px rgba(0,0,0,0.4);
      transition: transform 0.2s ease, box-shadow 0.2s ease;
    }
    .highlight-box:hover {
      transform: translateY(-3px);
      box-shadow: 0px 4px 12px rgba(0,0,0,0.5);
    }  
    .highlight-box a {
      color: #66ccff;
      text-decoration: none;
    } 
    .highlight-box a:hover {
      text-decoration: underline;
    }
    .highlight-box img {
      display: block;
      margin: 0 auto;
    }
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twemoji/14.0.2/twemoji.min.css">
    <script src="https://twemoji.maxcdn.com/v/latest/twemoji.min.js" crossorigin="anonymous"></script>
    <script>
    document.addEventListener("DOMContentLoaded", function() {
      twemoji.parse(document.body, { folder: 'svg', ext: '.svg' });
    });
  </script>
  .authors {
    display: inline-block;
    position: relative;
    font-weight: bold;
    color: #ffdf00;
    padding: 0.2em 0.4em;
    }
    .authors::after {
      content: '';
      position: absolute;
      top: -3px;
      left: -3px;
      width: calc(100% + 6px);
      height: calc(100% + 6px);
      background: radial-gradient(circle at center, rgba(255,255,0,0.7), transparent 70%);
      opacity: 0.6;
      border-radius: 4px;
      filter: blur(3px);
      z-index: -1;
    }
    .latest-cards {
      display: flex;
      flex-wrap: wrap;
      gap: 1.5rem;
      justify-content: center;
      margin: 2rem 0;
    }  
    .card {
      background: #ffffff;
      color: #333;
      padding: 1rem 1.5rem;
      border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      flex: 1 1 280px;
      max-width: 300px;
    } 
    .card h3 {
      margin-top: 0;
      color: #007acc;
    } 
    .card p {
      margin: 0.5rem 0;
    }

  </style>

  
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
