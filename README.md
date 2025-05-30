<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Excellent TV News</title>
  <style>
    /* Reset & basics */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body {
      background: #f5f5f5;
      color: #222;
      line-height: 1.6;
    }

    a {
      color: #007bff;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }

    /* Header */
    header {
      background-color: #0a1e3f;
      color: white;
      padding: 1rem 2rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
    }

    header h1 {
      font-size: 1.8rem;
      letter-spacing: 2px;
      font-weight: 700;
      cursor: default;
    }

    nav {
      margin-top: 0.5rem;
    }

    nav a {
      color: white;
      margin-left: 1.5rem;
      font-weight: 600;
      font-size: 1rem;
    }

    nav a:first-child {
      margin-left: 0;
    }

    /* Container */
    .container {
      max-width: 1100px;
      margin: 2rem auto;
      padding: 0 1rem;
    }

    /* Featured Article */
    .featured {
      background: white;
      border-radius: 8px;
      overflow: hidden;
      display: flex;
      flex-wrap: wrap;
      box-shadow: 0 2px 10px rgb(0 0 0 / 0.1);
      margin-bottom: 3rem;
    }

    .featured img {
      width: 100%;
      max-height: 350px;
      object-fit: cover;
      flex: 1 1 400px;
    }

    .featured-content {
      flex: 1 1 500px;
      padding: 1.5rem 2rem;
      display: flex;
      flex-direction: column;
      justify-content: center;
    }

    .featured-content h2 {
      font-size: 2rem;
      margin-bottom: 0.5rem;
      color: #0a1e3f;
    }

    .featured-content p {
      font-size: 1.1rem;
      color: #555;
      margin-bottom: 1rem;
    }

    .featured-content a {
      align-self: flex-start;
      background-color: #007bff;
      color: white;
      padding: 0.5rem 1.2rem;
      border-radius: 4px;
      font-weight: 600;
      transition: background-color 0.3s ease;
    }

    .featured-content a:hover {
      background-color: #0056b3;
    }

    /* News Grid */
    .news-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(280px,1fr));
      gap: 2rem;
    }

    .news-card {
      background: white;
      border-radius: 8px;
      box-shadow: 0 1px 6px rgb(0 0 0 / 0.1);
      overflow: hidden;
      display: flex;
      flex-direction: column;
      transition: transform 0.3s ease;
    }

    .news-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 4px 20px rgb(0 0 0 / 0.15);
    }

    .news-card img {
      width: 100%;
      height: 160px;
      object-fit: cover;
    }

    .news-content {
      padding: 1rem 1.2rem;
      flex-grow: 1;
      display: flex;
      flex-direction: column;
    }

    .news-content h3 {
      font-size: 1.25rem;
      color: #0a1e3f;
      margin-bottom: 0.5rem;
      flex-grow: 1;
    }

    .news-content p {
      font-size: 0.95rem;
      color: #666;
      margin-bottom: 1rem;
      flex-grow: 1;
    }

    .news-content a {
      align-self: flex-start;
      font-weight: 600;
      color: #007bff;
      border-bottom: 1px solid transparent;
      transition: border-bottom-color 0.3s ease;
    }

    .news-content a:hover {
      border-bottom-color: #007bff;
    }

    /* Footer */
    footer {
      background-color: #0a1e3f;
      color: white;
      text-align: center;
      padding: 1.5rem 1rem;
      margin-top: 4rem;
      font-size: 0.9rem;
    }

    /* Responsive adjustments */
    @media (max-width: 768px) {
      header {
        justify-content: center;
        text-align: center;
      }
      nav {
        width: 100%;
        margin-top: 0.5rem;
      }
      nav a {
        margin: 0 0.75rem;
        font-size: 0.95rem;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>Excellent TV News</h1>
    <nav>
      <a href="#">Home</a>
      <a href="#">World</a>
      <a href="#">Politics</a>
      <a href="#">Technology</a>
      <a href="#">Entertainment</a>
      <a href="#">Sports</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <main class="container">
    <section class="featured" aria-label="Featured News">
      <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=800&q=80" alt="Breaking news: technology innovation" />
      <div class="featured-content">
        <h2>Revolutionary Tech Innovation Unveiled Today</h2>
        <p>The world witnesses a groundbreaking technological breakthrough that promises to change the way we live and work, ushering a new era of possibilities.</p>
        <a href="#">Read More &raquo;</a>
      </div>
    </section>

    <section aria-label="Latest News">
      <div class="news-grid">
        <article class="news-card" tabindex="0">
          <img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?auto=format&fit=crop&w=800&q=80" alt="Political debate" />
          <div class="news-content">
            <h3>Political Debate Sparks National Conversation</h3>
            <p>Leaders from across the country engage in a heated debate addressing key policy issues affecting millions.</p>
            <a href="#">Read More &raquo;</a>
          </div>
        </article>

        <article class="news-card" tabindex="0">
          <img src="https://images.unsplash.com/photo-1510511459019-5dda7724fd87?auto=format&fit=crop&w=800&q=80" alt="Sports championship" />
          <div class="news-content">
            <h3>Local Team Wins Championship After Thrilling Match</h3>
            <p>In an epic showdown, the underdogs claim victory and bring home the coveted trophy.</p>
            <a href="#">Read More &raquo;</a>
          </div>
        </article>

        <article class="news-card" tabindex="0">
          <img src="https://images.unsplash.com/photo-1504384308090-c894fdcc538d?auto=format&fit=crop&w=800&q=80" alt="Entertainment gala" />
          <div class="news-content">
            <h3>Stars Shine Bright at Annual Entertainment Gala</h3>
            <p>Hollywood’s biggest names gather to celebrate achievements in film and television.</p>
            <a href="#">Read More &raquo;</a>
          </div>
        </article>

        <article class="news-card" tabindex="0">
          <img src="https://images.unsplash.com/photo-1497493292307-31c376b6e479?auto=format&fit=crop&w=800&q=80" alt="Global economic forum" />
          <div class="news-content">
            <h3>Global Economic Forum Addresses Climate Change Impact</h3>
            <p>World leaders and experts discuss sustainable solutions to mitigate economic risks from climate shifts.</p>
            <a href="#">Read More &raquo;</a>
          </div>
        </article>
      </div>
    </section>
  </main>

  <footer>
    &copy; 2025 Excellent TV News. All rights reserved.
  </footer>
</body>
</html>
