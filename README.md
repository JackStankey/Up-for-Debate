[index.html](https://github.com/user-attachments/files/26162435/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Up for Debate Tour</title>
  <meta name="description" content="Up for Debate is a multi-city live town hall tour featuring Scott Jennings and Van Jones." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@400;600;700&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="site-header">
    <div class="container nav-wrap">
      <a href="#top" class="brand">
        <img src="assets/page1.png" alt="Up for Debate logo graphic" class="brand-mark" />
        <span>Up for Debate</span>
      </a>
      <nav class="site-nav">
        <a href="#overview">Overview</a>
        <a href="#voices">Featured Voices</a>
        <a href="#headlines">Headlines</a>
        <a href="#tour">Tour Dates</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <main id="top">
    <section class="hero">
      <div class="hero-overlay"></div>
      <div class="container hero-content">
        <div class="eyebrow">Town Hall Tour • Fall 2026</div>
        <h1>Up for Debate</h1>
        <p class="hero-subhead">A live national tour bringing Scott Jennings and Van Jones together for a fast-paced, high-stakes conversation on the issues shaping American public life.</p>
        <div class="hero-actions">
          <a href="#tour" class="btn btn-primary">View Tour Dates</a>
          <a href="#headlines" class="btn btn-secondary">See Debate Topics</a>
        </div>
        <div class="hero-stats">
          <div class="stat-card">
            <span class="stat-number">6</span>
            <span class="stat-label">Tour stops</span>
          </div>
          <div class="stat-card">
            <span class="stat-number">2</span>
            <span class="stat-label">National voices</span>
          </div>
          <div class="stat-card">
            <span class="stat-number">1</span>
            <span class="stat-label">Audience verdict</span>
          </div>
        </div>
      </div>
    </section>

    <section id="overview" class="section section-dark">
      <div class="container split-section">
        <div>
          <p class="section-kicker">What the tour is</p>
          <h2>Substantive disagreement, live on stage.</h2>
          <p>Up for Debate is a multi-city live event series designed to model serious dialogue across political lines in the lead-up to the U.S. midterm elections. Each stop features a live audience, a moderator, structured issue blocks, and audience participation.</p>
          <p>Rather than partisan theater, the format is built around informed disagreement. Guests make their case, challenge each other directly, answer audience questions, and let the crowd decide who made the stronger argument on each topic.</p>
        </div>
        <div class="info-panel">
          <h3>Event format</h3>
          <ul class="timeline-list">
            <li><span>5:00 PM</span> Doors open</li>
            <li><span>6:00 PM</span> Discussion begins</li>
            <li><span>7:00 PM</span> Audience Q&amp;A</li>
            <li><span>7:30 PM</span> Event concludes</li>
          </ul>
          <div class="badge-row">
            <span class="pill">Live audience</span>
            <span class="pill">Moderated format</span>
            <span class="pill">Issue-by-issue voting</span>
          </div>
        </div>
      </div>
    </section>

    <section id="voices" class="section">
      <div class="container">
        <p class="section-kicker">Featured voices</p>
        <h2>Two national commentators. Opposite ideological lanes.</h2>
        <div class="speaker-grid">
          <article class="speaker-card left-card">
            <img src="assets/van-jones.png" alt="Van Jones" class="speaker-image" />
            <div class="speaker-copy">
              <span class="speaker-tag">Left-of-center perspective</span>
              <h3>Van Jones</h3>
              <p>Van Jones is a CNN host, political commentator, bestselling author, and longtime advocate on criminal justice reform, human rights, and systemic change. He previously served as a senior advisor to President Barack Obama.</p>
            </div>
          </article>
          <article class="speaker-card right-card">
            <img src="assets/scott-jennings.png" alt="Scott Jennings" class="speaker-image" />
            <div class="speaker-copy">
              <span class="speaker-tag">Conservative perspective</span>
              <h3>Scott Jennings</h3>
              <p>Scott Jennings is a CNN senior political commentator, Republican strategist, and co-founder of RunSwitch. A former special assistant to President George W. Bush, he is known for defending conservative policy positions in high-profile TV debates.</p>
            </div>
          </article>
        </div>
      </div>
    </section>

    <section id="headlines" class="section section-dark issue-section">
      <div class="container">
        <p class="section-kicker">Major headlines from the deck</p>
        <h2>The issues expected to drive the room.</h2>
        <p class="section-intro">These sections track the core topics outlined in the presentation deck. Each includes a short quote card for Scott Jennings and Van Jones reflecting the contrasting arguments likely to shape the conversation.</p>
        <div id="issues-grid" class="issues-grid"></div>
      </div>
    </section>

    <section id="tour" class="section">
      <div class="container">
        <div class="tour-header">
          <div>
            <p class="section-kicker">Tour route</p>
            <h2>Updated dates and locations</h2>
          </div>
          <div class="tour-note">Dates and markets updated from the latest tour schedule document.</div>
        </div>
        <div class="map-wrap">
          <div id="tour-map" aria-label="Map of Up for Debate tour stops"></div>
        </div>
        <div id="tour-stops" class="tour-stops"></div>
      </div>
    </section>

    <section class="section cta-section">
      <div class="container cta-box">
        <div>
          <p class="section-kicker">Why it stands out</p>
          <h2>A political event built for live reaction.</h2>
          <p>The tour is positioned as a national town hall experience: recognizable talent, culturally relevant topics, audience participation, and a visual split-screen identity that mirrors the debate itself.</p>
        </div>
        <a href="#tour" class="btn btn-primary">Track the Tour</a>
      </div>
    </section>
  </main>

  <footer id="contact" class="site-footer">
    <div class="container footer-grid">
      <div>
        <h3>Up for Debate</h3>
        <p>Town Hall Tour featuring Scott Jennings and Van Jones.</p>
      </div>
      <div>
        <h4>Deck contacts</h4>
        <p>Jon Venison — EVP, Head of Productions</p>
        <p>William Moss — Director, Business Development</p>
        <p>Brian Jacobs — Senior Vice President, Broadcasting</p>
      </div>
      <div>
        <h4>Built from</h4>
        <p>Tour schedule image and the <em>Up For Debate Overview</em> presentation deck.</p>
      </div>
    </div>
  </footer>

  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
  <script src="style.js"></script>
</body>
</html>
