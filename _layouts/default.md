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
  </style>
</head>
<body>
  <header>
    <nav>
      <a href="/">Home</a> |
      <a href="/about/">About</a> |
      <a href="/team/">Team</a> |
      <a href="/team/">Transients!!!</a> |
      <a href="/News/">News</a> |
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
