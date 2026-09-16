<p align="center">
  <svg width="100%" height="320" viewBox="0 0 800 320" xmlns="http://www.w3.org/2000/svg">
    <style>
      @import url('https://fonts.googleapis.com/css2?family=Cinzel:wght@600&amp;display=swap');

      .bg {
        fill: #080808;
      }

      /* Glowing Red Silhouette Styling */
      .fox-art {
        fill: #ff3311;
        filter: drop-shadow(0 0 12px rgba(255, 50, 15, 0.6))
                drop-shadow(0 0 25px rgba(255, 20, 0, 0.3));
        animation: pulseGlow 4s ease-in-out infinite alternate;
      }

      /* Text Styling */
      .name-text {
        font-family: 'Cinzel', serif;
        font-size: 32px;
        fill: #ff4522;
        letter-spacing: 4px;
        filter: drop-shadow(0 0 8px rgba(255, 60, 20, 0.7));
      }

      /* Smoke / Fog Particle Animations */
      .smoke-1 {
        fill: rgba(255, 60, 20, 0.15);
        filter: blur(12px);
        animation: driftSmoke1 8s linear infinite;
      }

      .smoke-2 {
        fill: rgba(200, 30, 10, 0.12);
        filter: blur(15px);
        animation: driftSmoke2 11s linear infinite;
      }

      @keyframes pulseGlow {
        0% { opacity: 0.85; transform: scale(1); }
        100% { opacity: 1; transform: scale(1.01); transform-origin: 250px 160px; }
      }

      @keyframes driftSmoke1 {
        0% { transform: translate(-30px, 20px) scale(0.9); opacity: 0; }
        30% { opacity: 0.6; }
        70% { opacity: 0.4; }
        100% { transform: translate(120px, -40px) scale(1.3); opacity: 0; }
      }

      @keyframes driftSmoke2 {
        0% { transform: translate(0px, 30px) scale(1); opacity: 0; }
        40% { opacity: 0.5; }
        80% { opacity: 0.3; }
        100% { transform: translate(150px, -50px) scale(1.5); opacity: 0; }
      }
    </style>

    <!-- Background -->
    <rect width="800" height="320" class="bg" rx="12" />

    <!-- Ambient Smoke Layers behind/around the art -->
    <circle cx="200" cy="200" r="60" class="smoke-1" />
    <circle cx="320" cy="140" r="80" class="smoke-2" />
    <circle cx="450" cy="180" r="70" class="smoke-1" style="animation-delay: -4s;" />

    <!-- Fox Head Silhouette Path (Inspired by your reference art) -->
    <g transform="translate(110, 40)">
      <path class="fox-art" d="M185,190 C160,175 130,150 115,120 C112,112 113,105 118,95 C125,75 135,30 140,15 C142,10 148,8 152,12 C162,25 178,65 188,90 C195,85 205,65 212,45 C215,35 220,30 225,32 C230,35 233,42 232,50 C228,72 218,105 212,120 C210,126 210,132 214,136 C225,148 248,168 275,182 C295,192 310,205 320,215 C325,220 322,230 315,232 C280,240 220,245 185,190 Z" />
      
      <!-- Eye detail cutout for dark contrast -->
      <polygon points="172,115 182,120 176,124" fill="#080808" />
    </g>

    <!-- Foreground Smoke Sweeps -->
    <ellipse cx="380" cy="210" rx="90" ry="35" class="smoke-2" style="animation-delay: -2s;" />
    <ellipse cx="500" cy="160" rx="110" ry="40" class="smoke-1" style="animation-delay: -5s;" />

    <!-- Name & Typography -->
    <text x="460" y="150" class="name-text">KYRILLOS WAHID</text>
    <text x="462" y="185" font-family="'Cinzel', serif" font-size="14px" fill="#772211" letter-spacing="6px">SOFTWARE DEVELOPER</text>
  </svg>
</p>
