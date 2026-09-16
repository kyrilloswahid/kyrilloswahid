<p align="center">
  <svg width="650" height="120" viewBox="0 0 650 120" xmlns="http://w3.org">
    <style>
      .smoke-text {
        font: bold 40px 'Segoe UI', -apple-system, sans-serif;
        fill: #ffffff;
        letter-spacing: 4px;
      }
      .smoke-blur {
        font: bold 40px 'Segoe UI', -apple-system, sans-serif;
        fill: none;
        stroke: #ffffff;
        stroke-width: 2.5;
        letter-spacing: 4px;
        opacity: 0.6;
        filter: url(#smoke-effect);
        animation: smokeDrift 6s infinite ease-in-out;
      }
      @keyframes smokeDrift {
        0% { transform: translate(0, 0); opacity: 0.5; }
        50% { transform: translate(5px, -6px); opacity: 0.15; }
        100% { transform: translate(0, 0); opacity: 0.5; }
      }
    </style>
    <defs>
      <filter id="smoke-effect">
        <feGaussianBlur stdDeviation="6" />
      </filter>
    </defs>
    <!-- Background smoking blur layer -->
    <text x="50%" y="50%" dominant-baseline="middle" text-anchor="middle" class="smoke-blur">Kyrillos Wahid</text>
    <!-- Sharp foreground layer -->
    <text x="50%" y="50%" dominant-baseline="middle" text-anchor="middle" class="smoke-text">Kyrillos Wahid</text>
  </svg>
</p>
