<p align="center">
  <svg width="100%" height="240" viewBox="0 0 800 240" xmlns="http://www.w3.org/2000/svg">
    <style>
      @import url('https://fonts.googleapis.com/css2?family=Cinzel:wght@500;700&amp;family=Inter:wght@300&amp;display=swap');

      .bg {
        fill: #050505;
      }

      /* Glowing Red Accents inspired by the art */
      .glow-accent {
        fill: #ff2a00;
        filter: drop-shadow(0 0 15px rgba(255, 42, 0, 0.6))
                drop-shadow(0 0 30px rgba(200, 20, 0, 0.3));
        animation: subtlePulse 4s ease-in-out infinite alternate;
      }

      /* Typography */
      .name-text {
        font-family: 'Cinzel', serif;
        font-weight: 700;
        font-size: 34px;
        fill: #ff3b19;
        letter-spacing: 5px;
        filter: drop-shadow(0 0 10px rgba(255, 40, 10, 0.5));
      }

      .quote-text {
        font-family: 'Inter', sans-serif;
        font-weight: 300;
        font-size: 13px;
        fill: #8a8a8a;
        letter-spacing: 3px;
        text-transform: uppercase;
      }

      /* Deep Smoke Animations */
      .smoke-deep {
        fill: rgba(180, 20, 5, 0.08);
        filter: blur(18px);
        animation: driftDeep 12s linear infinite;
      }

      .smoke-mid {
        fill: rgba(255, 60, 20, 0.12);
        filter: blur(14px);
        animation: driftMid 8s linear infinite;
      }

      .smoke-wisps {
        fill: rgba(255, 255, 255, 0.03);
        filter: blur(8px);
        animation: driftWisps 6s ease-in-out infinite alternate;
      }

      @keyframes subtlePulse {
        0% { opacity: 0.8; transform: scale(1); }
        100% { opacity: 1; transform: scale(1.01); transform-origin: 100px 120px; }
      }

      @keyframes driftDeep {
        0% { transform: translate(-40px, 10px) scale(0.9); opacity: 0; }
        30% { opacity: 0.7; }
        70% { opacity: 0.5; }
        100% { transform: translate(180px, -20px) scale(1.4); opacity: 0; }
      }

      @keyframes driftMid {
        0% { transform: translate(10px, 30px) scale(0.8); opacity: 0; }
        40% { opacity: 0.6; }
        80% { opacity: 0.3; }
        100% { transform: translate(-120px, -30px) scale(1.3); opacity: 0; }
      }

      @keyframes driftWisps {
        0% { transform: translate(0, 5px); opacity: 0.2; }
        100% { transform: translate(40px, -15px); opacity: 0.6; }
      }
    </style>

    <!-- Deep Background -->
    <rect width="800" height="240" class="bg" rx="10" />

    <!-- Ambient Background Smoke Layers -->
    <circle cx="150" cy="120" r="90" class="smoke-deep" />
    <circle cx="400" cy="100" r="110" class="smoke-mid" style="animation-delay: -4s;" />
    <circle cx="650" cy="140" r="80" class="smoke-deep" style="animation-delay: -7s;" />

    <!-- Abstract Minimal Accent Lines / Vibe from the Fox Art -->
    <g class="glow-accent" transform="translate(60, 75)">
      <!-- Sleek sharp lines representing the fox's silhouette contour & ears -->
      <polygon points="40,60 55,10 75,45 90,15 105,70" />
      <path d="M 20,80 Q 60,65 120,75" stroke="#ff2a00" stroke-width="3" fill="none" opacity="0.8" />
    </g>

    <!-- Foreground Smoke Rolling Across -->
    <ellipse cx="300" cy="150" rx="140" ry="30" class="smoke-mid" style="animation-delay: -2s;" />
    <ellipse cx="550" cy="110" rx="120" ry="25" class="smoke-wisps" style="animation-delay: -1s;" />

    <!-- Name and Quote/Job Title Grouped Centrally -->
    <g transform="translate(240, 0)">
      <text x="0" y="115" class="name-text">KYRILLOS WAHID</text>
      <text x="2" y="148" class="quote-text">Software Engineer &bull; Creator</text>
    </g>
  </svg>
</p>
