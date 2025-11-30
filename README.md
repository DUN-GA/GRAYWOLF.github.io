<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>GRAYWOLF — Modern Urban Goods</title>
  <meta name="description" content="GRAYWOLF — crafted urban goods and apparel." />
  <link rel="stylesheet" href="styles.css" />
</head>

<body>
  <div class="site" role="main">

    <!-- HEADER -->
    <header>
      <a class="logo" href="#">
        <svg viewBox="0 0 100 100" role="img" aria-label="GRAYWOLF logo" xmlns="http://www.w3.org/2000/svg">
          <defs>
            <linearGradient id="g" x1="0" x2="1">
              <stop offset="0" stop-color="#F47C3C"/>
              <stop offset="1" stop-color="#F27D50"/>
            </linearGradient>
          </defs>
          <rect width="100" height="100" rx="18" fill="#071022"/>
          <path d="M24 68 C40 84, 60 84, 76 68 L68 50 C60 56, 40 56,32 50 Z" fill="url(#g)"/>
          <text x="50" y="55" text-anchor="middle" font-family="Arial, sans-serif" font-weight="700" font-size="24" fill="#fff">GW</text>
        </svg>

        <span class="brand">
          <span class="name">GRAYWOLF</span>
          <span class="tag">urban goods & apparel</span>
        </span>
      </a>

      <nav>
        <a href="#shop">Shop</a>
        <a href="#about">About</a>
        <a href="#collections">Collections</a>
        <a href="#contact" class="primary">Contact</a>
      </nav>
    </header>

    <!-- HERO -->
    <section class="hero">
      <div>
        <div class="pill">New — Fall / Winter 2025</div>
        <h1>GRAYWOLF — bold, sustainable urban goods</h1>
        <p>Design-forward apparel and accessories built for the city.</p>

        <div class="hero-actions">
          <button class="btn cta" onclick="location.href='#shop'">Shop the collection</button>
          <button class="btn ghost" onclick="location.href='#about'">Learn about GRAYWOLF</button>
        </div>

        <div class="info-row">
          <span class="muted-small">Free shipping over $75</span>
          <span class="muted-small">Sustainably sourced fabrics</span>
        </div>
      </div>

      <aside class="hero-card">
        <div class="product-thumb">
          <img src="https://images.unsplash.com/photo-1541099649105-f69ad21f3246?q=80&w=1200&auto=format&fit=crop&crop=entropy" alt="Featured jacket">
        </div>

        <div class="product-meta">
          <div>
            <div class="title">GRAYWOLF Field Jacket</div>
            <div class="muted-small">Lightweight, water-resistant</div>
          </div>
          <div class="price-box">
            <div class="price">$149</div>
            <div class="muted-small">Limited drop</div>
          </div>
        </div>
      </aside>
    </section>

    <!-- FEATURES -->
    <section>
      <div class="features">
        <div class="feature">
          <h3>Quality materials</h3>
          <p>Durable, low-impact fabrics tested for longevity.</p>
        </div>

        <div class="feature">
          <h3>Urban-first design</h3>
          <p>Functional pockets and silhouettes built for city life.</p>
        </div>

        <div class="feature">
          <h3>Conscious production</h3>
          <p>Small-batch manufacturing with reduced waste.</p>
        </div>
      </div>
    </section>

    <!-- PRODUCTS -->
    <section id="shop">
      <h2>Featured products</h2>
      <div class="products">

        <article class="card">
          <img src="https://images.unsplash.com/photo-1530845640667-2e0b269a9d25?q=80&w=1400&auto=format&fit=crop&crop=entropy" alt="Hoodie">
          <div class="meta">
            <div>
              <div class="title">Minimal Hoodie</div>
              <div class="muted-small">Unisex — soft fleece</div>
            </div>
            <div class="price">$69</div>
          </div>
        </article>

        <article class="card">
          <img src="https://images.unsplash.com/photo-1520975688374-2c4d2b09e9b6?q=80&w=1400&auto=format&fit=crop&crop=entropy" alt="Tote Bag">
          <div class="meta">
            <div>
              <div class="title">City Tote</div>
              <div class="muted-small">Heavy-duty canvas — 18L</div>
            </div>
            <div class="price">$39</div>
          </div>
        </article>

        <article class="card">
          <img src="https://images.unsplash.com/photo-1519741491602-3c5a6b11c7e0?q=80&w=1400&auto=format&fit=crop&crop=entropy" alt="Cap">
          <div class="meta">
            <div>
              <div class="title">Everyday Cap</div>
              <div class="muted-small">Low-profile — adjustable</div>
            </div>
            <div class="price">$24</div>
          </div>
        </article>

      </div>
    </section>

    <!-- ABOUT + TESTIMONIALS -->
    <section id="about" class="about-wrap">
      <div>
        <h2>About GRAYWOLF</h2>
        <p class="muted-small">
          GRAYWOLF is a collective designing purposeful goods for modern city life.
        </p>

        <div class="testimonials">
          <blockquote class="testimonial">
            <strong>“Best jacket I've owned. Lightweight and weather-proof.”</strong>
            <div class="muted-small">— Alex</div>
          </blockquote>

          <blockquote class="testimonial">
            <strong>“The tote is my everyday carry. Stylish & functional.”</strong>
            <div class="muted-small">— Priya</div>
          </blockquote>
        </div>
      </div>

      <aside class="signup-box">
        <h3>Join the pack</h3>
        <p class="muted-small">Early access to drops and design stories.</p>

        <form id="signup-form" onsubmit="event.preventDefault(); signup()">
          <label class="muted-small" for="email">Email</label>
          <input id="email" type="email" required placeholder="you@example.com" />

          <button class="btn cta" type="submit">Join</button>
        </form>

        <div id="signup-msg" class="muted-small msg"></div>
      </aside>
    </section>

    <!-- CONTACT -->
    <section id="contact" class="contact-wrap">
      <div>
        <h2>Contact GRAYWOLF</h2>
        <form id="contact-form" onsubmit="event.preventDefault(); sendContact()">
          <label class="muted-small" for="name">Name</label>
          <input id="name" type="text" required />

          <label class="muted-small" for="email2">Email</label>
          <input id="email2" type="email" required />

          <label class="muted-small" for="message">Message</label>
          <textarea id="message" rows="4" required></textarea>

          <button class="btn cta" type="submit">Send message</button>
        </form>

        <div id="contact-msg" class="muted-small msg"></div>
      </div>

      <aside class="map-box">
        <h4>Visit / Wholesale</h4>
        <p class="muted-small">hello@graywolf.example</p>

        <img class="map-img" src="https://images.unsplash.com/photo-1508057198894-247b23fe5ade?q=80&w=1200&auto=format&fit=crop&crop=entropy" alt="Map placeholder" />
      </aside>
    </section>

    <!-- FOOTER -->
    <footer>
      <div>© GRAYWOLF — Built with care.</div>
      <div class="footer-links">
        <a href="#">Privacy</a>
        <a href="#">Terms</a>
      </div>
    </footer>

  </div>

  <script src="app.js"></script>
</body>
</html>
