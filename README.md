<div align="center">
<style>
@import url("https://fonts.googleapis.com/css?family=Raleway:400,400i,700");

*, *::before, *::after {
    padding: 0;
    margin: 0 auto;
    box-sizing: border-box;
}

.content {
  font-family: Raleway, sans-serif;
  background-color: #000;
  color: #fff;
  font-size: 24px;
  width: 95%;
  max-width: 40ch;
  padding: 3em 1em;
}

.marquee {
  position: relative;
  width: 100%;
  height: 2em;
  font-size: 5em;
  display: grid;
  place-items: center;
  overflow: hidden;
}

.marquee_text {
  position: absolute;
  min-width: 100%;
  white-space: nowrap;
  animation: marquee 16s infinite linear;
}

@keyframes marquee {
  from { translate: 70%; }
  to { translate: -70%; }
}

.marquee_blur {
  position: absolute;
  inset: 0;
  display: grid;
  place-items: center;
  background-color: black;
  background-image:
    linear-gradient(to right, white, 1rem, transparent 50%),
    linear-gradient(to left, white, 1rem, transparent 50%);
  filter: contrast(15);
}

.marquee_blur p {
  filter: blur(0.07em);
}

.marquee_clear {
  position: absolute;
  inset: 0;
  display: grid;
  place-items: center;
}

.text {
  margin-block: 2em;
}
</style>

<div class="content">
  <div class="marquee">
    <div class="marquee_blur" aria-hidden="true">
      <p class="marquee_text">Kyrillos Wahid</p>
    </div>
    <div class="marquee_clear">
      <p class="marquee_text">Kyrillos Wahid</p>
    </div>
  </div>

  <p class="text">
    Motivation gets you started,
Habit keeps you going.
  </p>
</div>
</div>
