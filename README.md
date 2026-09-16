<p align="center">
  <svg width="500" height="100" viewBox="0 0 500 100" xmlns="http://w3.org">
    <style>
      .smoke-text {
        font: bold 45px 'Segoe UI', sans-serif;
        fill: #ffffff;
        letter-spacing: 5px;
      }
      .smoke-blur {
        font: bold 45px 'Segoe UI', sans-serif;
        fill: none;
        stroke: #ffffff;
        stroke-width: 2;
        letter-spacing: 5px;
        opacity: 0.6;
        filter: url(#blur-effect);
        animation: drift 5s infinite linear;
      }
      @keyframes drift {
        0% { transform: translate(0, 0); opacity: 0.6; }
        50% { transform: translate(3px, -3px); opacity: 0.2; filter: blur(6px); }
        100% { transform: translate(0, 0); opacity: 0.6; }
      }
    </style>
    <defs>
      <filter id="blur-effect">
        <feGaussianBlur stdDeviation="4" />
      </filter>
    </defs>
    <!-- Background blurred smoke layer -->
    <text x="50%" y="60%" dominant-baseline="middle" text-anchor="middle" class="smoke-blur">YOUR NAME</text>
    <!-- Sharp foreground text -->
    <text x="50%" y="60%" dominant-baseline="middle" text-anchor="middle" class="smoke-text">YOUR NAME</text>
  </svg>
</p>
