<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy 13th Birthday Maheen</title>
  <style>
    :root {
      --bg1: #f9dfe9;
      --bg2: #f5d5e6;
      --bg3: #f1d5ff;
      --bg4: #dff5ff;
      --rose: #e8689f;
      --rose2: #d9488d;
      --pink: #f9b9d4;
      --lavender: #cbb9ff;
      --blue: #8ad3ff;
      --gold: #ffd86b;
      --peach: #ffd3ad;
      --text: #4b2a3d;
      --paper: #fffafc;
      --white: #ffffff;
      --shadow: rgba(84, 35, 59, 0.18);
    }

    * { box-sizing: border-box; }

    html, body {
      margin: 0;
      width: 100%;
      min-height: 100%;
      overflow-x: hidden;
      font-family: "Trebuchet MS", "Segoe UI", sans-serif;
      background: linear-gradient(180deg, #fbe7f1 0%, #f6d8ea 28%, #f4d6ef 100%);
      color: var(--text);
    }

    body {
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .scene {
      position: relative;
      width: 100%;
      min-height: 100vh;
      overflow: hidden;
      display: flex;
      align-items: center;
      justify-content: center;
      background:
        radial-gradient(circle at 15% 12%, rgba(255,255,255,0.7), transparent 12%),
        radial-gradient(circle at 72% 10%, rgba(255,255,255,0.45), transparent 11%),
        linear-gradient(180deg, rgba(255,255,255,0.12), rgba(255,255,255,0)),
        linear-gradient(180deg, var(--bg1) 0%, var(--bg2) 35%, var(--bg3) 68%, var(--bg4) 100%);
    }

    .scene::before {
      content: "";
      position: absolute;
      inset: 0;
      background:
        radial-gradient(ellipse at 20% 70%, rgba(255,255,255,0.75), transparent 31%),
        radial-gradient(ellipse at 78% 65%, rgba(255,255,255,0.65), transparent 28%),
        radial-gradient(ellipse at 50% 92%, rgba(255,255,255,0.4), transparent 25%);
      filter: blur(28px);
      pointer-events: none;
      opacity: 0.9;
    }

    .content {
      position: relative;
      z-index: 3;
      width: min(96vw, 980px);
      padding: 52px 18px 120px;
      text-align: center;
      animation: rise 0.9s ease both;
    }

    @keyframes rise {
      from { opacity: 0; transform: translateY(16px) scale(0.98); }
      to { opacity: 1; transform: translateY(0) scale(1); }
    }

    h1 {
      margin: 0 0 10px;
      font-size: clamp(2.3rem, 5vw, 4.8rem);
      line-height: 1.08;
      letter-spacing: 0.02em;
      color: #fff;
      text-shadow:
        0 4px 0 rgba(181, 93, 140, 0.88),
        0 10px 25px rgba(74, 44, 58, 0.2);
      animation: floatTitle 3.5s ease-in-out infinite alternate;
    }

    @keyframes floatTitle {
      0% { transform: translateY(0) rotate(-0.3deg); }
      100% { transform: translateY(-7px) rotate(0.45deg); }
    }

    .date {
      display: inline-block;
      margin-bottom: 20px;
      padding: 10px 18px;
      border-radius: 999px;
      background: rgba(255,255,255,0.56);
      border: 1px solid rgba(255,255,255,0.8);
      color: #86586b;
      font-size: clamp(0.8rem, 1.8vw, 1rem);
      letter-spacing: 0.22em;
      font-weight: 800;
      box-shadow: 0 8px 22px rgba(98, 42, 74, 0.09);
      backdrop-filter: blur(8px);
    }

    .photo-frame {
      position: relative;
      width: min(100%, 620px);
      margin: 0 auto;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: clamp(14px, 3vw, 28px);
      padding: 22px clamp(16px, 3vw, 30px);
      border-radius: 28px;
      background: rgba(255, 249, 252, 0.62);
      border: 2px solid rgba(255,255,255,0.9);
      box-shadow:
        0 18px 52px rgba(111, 53, 76, 0.15),
        inset 0 0 0 6px rgba(255,255,255,0.25);
      backdrop-filter: blur(10px);
      animation: frameFloat 5s ease-in-out infinite;
    }

    @keyframes frameFloat {
      0%,100% { transform: translateY(0) rotate(-0.4deg); }
      50% { transform: translateY(-10px) rotate(0.4deg); }
    }

    .photo-frame::before {
      content: "";
      position: absolute;
      inset: 10px;
      border: 1px dashed rgba(216, 125, 159, 0.7);
      border-radius: 18px;
      pointer-events: none;
    }

    .heart {
      position: absolute;
      right: 18px;
      top: -16px;
      color: #ea5d96;
      font-size: 2rem;
      filter: drop-shadow(0 4px 6px rgba(135,60,89,0.18));
      animation: heartBeat 1.7s ease-in-out infinite;
    }

    @keyframes heartBeat {
      0%,100% { transform: scale(1); }
      50% { transform: scale(1.18); }
    }

    .polaroid {
      width: min(39%, 210px);
      aspect-ratio: 1;
      overflow: hidden;
      border: 7px solid rgba(255,255,255,0.95);
      border-radius: 18px;
      background: #fff;
      box-shadow: 0 10px 22px rgba(68, 34, 49, 0.15);
      animation: wiggle 6s ease-in-out infinite;
    }

    .polaroid:nth-of-type(2) { animation-delay: -3s; }

    @keyframes wiggle {
      0%,100% { transform: rotate(-3deg) translateY(0); }
      50% { transform: rotate(3deg) translateY(-5px); }
    }

    .polaroid svg {
      display: block;
      width: 100%;
      height: 100%;
    }

    .hint {
      margin: 22px 0 0;
      color: #7a5267;
      font-size: clamp(0.82rem, 1.8vw, 1rem);
      font-weight: 700;
      letter-spacing: 0.04em;
      text-shadow: 0 1px 10px rgba(255,255,255,0.7);
    }

    .balloons, .stars {
      position: absolute;
      inset: 0;
      z-index: 2;
      pointer-events: none;
    }

    .balloon {
      position: absolute;
      bottom: -110px;
      width: 52px;
      height: 70px;
      border-radius: 50% 50% 48% 48%;
      box-shadow: inset -8px -8px 0 rgba(255,255,255,0.22);
      animation: balloonFloat 7s ease-in-out infinite;
    }

    .balloon::before {
      content: "";
      position: absolute;
      left: 50%;
      bottom: -98px;
      width: 2px;
      height: 98px;
      background: rgba(90, 60, 77, 0.42);
      transform: translateX(-50%);
    }

    .balloon::after {
      content: "";
      position: absolute;
      left: 10px;
      top: 12px;
      width: 14px;
      height: 14px;
      border-radius: 50%;
      background: rgba(255,255,255,0.36);
    }

    .balloon:nth-child(1) { left: 5%; background: linear-gradient(#ff9bc9, #ff5da5); }
    .balloon:nth-child(2) { left: 20%; background: linear-gradient(#ffe49f, #ffb625); animation-delay: -1.7s; }
    .balloon:nth-child(3) { left: 76%; background: linear-gradient(#b7e7ff, #58baf7); animation-delay: -3s; }
    .balloon:nth-child(4) { left: 89%; background: linear-gradient(#d7c7ff, #8f73f4); animation-delay: -4.2s; }

    @keyframes balloonFloat {
      0%,100% { transform: translateY(0) rotate(-2deg); }
      50% { transform: translateY(-20px) rotate(4deg); }
    }

    .sparkle {
      position: absolute;
      top: -28px;
      left: var(--x);
      color: var(--c);
      opacity: 0;
      font-size: var(--s);
      text-shadow: 0 0 12px rgba(255,255,255,0.9);
      animation: fall var(--dur) linear var(--delay) infinite;
    }

    @keyframes fall {
      0% {
        opacity: 0;
        transform: translate(0, -20px) rotate(0deg);
      }
      12% {
        opacity: 0.9;
      }
      100% {
        opacity: 0;
        transform: translate(var(--drift), 118vh) rotate(260deg);
      }
    }

    .cake-button {
      position: absolute;
      left: 8%;
      bottom: 4%;
      z-index: 6;
      width: 90px;
      height: 90px;
      border: 2px solid rgba(255,255,255,0.85);
      border-radius: 50%;
      background: rgba(255,255,255,0.12);
      box-shadow: 0 0 0 0 rgba(255,255,255,0.7);
      cursor: pointer;
      animation: cakePulse 2.2s ease-out infinite;
      transition: transform 220ms ease, background 220ms ease;
    }

    .cake-button:hover {
      transform: scale(1.05);
      background: rgba(255,255,255,0.18);
    }

    .cake-button:focus-visible {
      outline: 3px solid #fff;
      outline-offset: 5px;
    }

    @keyframes cakePulse {
      0% { box-shadow: 0 0 0 0 rgba(255,255,255,0.7); }
      70% { box-shadow: 0 0 0 18px rgba(255,255,255,0); }
      100% { box-shadow: 0 0 0 0 rgba(255,255,255,0); }
    }

    .cake-label {
      position: absolute;
      left: 4.2%;
      bottom: calc(4% + 94px);
      z-index: 6;
      padding: 7px 12px;
      border-radius: 999px;
      background: rgba(255,250,252,0.92);
      color: #865767;
      font-size: 0.75rem;
      letter-spacing: 0.06em;
      font-weight: 800;
      animation: labelBob 2s ease-in-out infinite;
    }

    @keyframes labelBob {
      50% { transform: translateY(-4px); }
    }

    .tiny-cake {
      position: absolute;
      left: 50%;
      top: 50%;
      width: 30px;
      height: 28px;
      transform: translate(-50%, -50%);
      pointer-events: none;
    }

    .tiny-cake .cake-top {
      position: absolute;
      left: 4px;
      right: 4px;
      top: 0;
      height: 10px;
      background: linear-gradient(180deg, #fefefe, #f9e7ef);
      border: 2px solid rgba(82, 49, 62, 0.8);
      border-bottom: none;
      border-radius: 4px 4px 0 0;
    }

    .tiny-cake .cake-body {
      position: absolute;
      left: 6px;
      right: 6px;
      bottom: 6px;
      height: 16px;
      background: linear-gradient(180deg, #fffdfd, #fbe0ea);
      border: 2px solid rgba(82, 49, 62, 0.8);
      border-radius: 4px;
    }

    .tiny-cake .cherry {
      position: absolute;
      left: 12px;
      top: -4px;
      width: 7px;
      height: 7px;
      border-radius: 50%;
      background: #f23c6b;
      box-shadow: 0 0 0 2px rgba(255,255,255,0.6);
    }

    .tiny-cake .candle {
      position: absolute;
      left: 21px;
      top: -16px;
      width: 3px;
      height: 12px;
      background: #ffef9c;
      border-radius: 3px;
      box-shadow: 0 0 0 1px rgba(89, 44, 56, 0.35);
    }

    .tiny-cake .flame {
      position: absolute;
      left: 19px;
      top: -18px;
      width: 7px;
      height: 9px;
      background: linear-gradient(180deg, #ffd75b, #ff8a00);
      border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
      transform: rotate(-15deg);
      box-shadow: 0 0 8px rgba(255, 172, 40, 0.7);
    }

    .overlay {
      position: fixed;
      inset: 0;
      z-index: 30;
      display: grid;
      place-items: center;
      padding: 18px;
      background: rgba(62, 35, 48, 0.42);
      opacity: 0;
      visibility: hidden;
      transition: opacity 260ms ease, visibility 260ms ease;
      backdrop-filter: blur(7px);
    }

    .overlay.open {
      opacity: 1;
      visibility: visible;
    }

    .letter-box {
      position: relative;
      width: min(92vw, 630px);
      max-height: 82vh;
      overflow: auto;
      padding: clamp(26px, 5vw, 46px);
      border-radius: 28px;
      background: linear-gradient(135deg, #fffafd 0%, #fff0f5 100%);
      border: 2px solid rgba(255,255,255,0.92);
      box-shadow: 0 28px 90px rgba(87, 39, 63, 0.25);
      transform: translateY(24px) scale(0.96);
      transition: transform 340ms cubic-bezier(.2,.8,.2,1);
    }

    .overlay.open .letter-box {
      transform: translateY(0) scale(1);
    }

    .close-btn {
      position: absolute;
      top: 12px;
      right: 14px;
      width: 38px;
      height: 38px;
      border: 0;
      border-radius: 50%;
      background: #f8dfe9;
      color: #785164;
      font-size: 1.45rem;
      cursor: pointer;
      transition: transform 180ms ease, background 180ms ease;
    }

    .close-btn:hover {
      transform: rotate(90deg);
      background: #f0c9d9;
    }

    .letter-box h2 {
      margin: 0 28px 18px;
      text-align: center;
      color: var(--rose2);
      font-size: clamp(1.6rem, 4.3vw, 2.5rem);
      line-height: 1.15;
    }

    .letter-box p {
      margin: 0;
      color: #4b2a3d;
      font-size: clamp(1rem, 2.2vw, 1.18rem);
      line-height: 1.9;
      font-weight: 600;
      white-space: pre-line;
    }

    @media (max-width: 640px) {
      .content {
        padding-bottom: 120px;
      }
      .photo-frame {
        width: min(100%, 460px);
      }
      .polaroid {
        width: 42%;
      }
      .cake-button {
        width: 74px;
        height: 74px;
        left: 8%;
        bottom: 3.5%;
      }
      .cake-label {
        left: 4%;
        bottom: calc(3.5% + 80px);
      }
    }
  </style>
</head>
<body>
  <main class="scene">
    <div class="balloons" aria-hidden="true">
      <div class="balloon"></div>
      <div class="balloon"></div>
      <div class="balloon"></div>
      <div class="balloon"></div>
    </div>

    <div class="stars" id="stars" aria-hidden="true"></div>

    <section class="content">
      <h1>HAPPY 13th BIRTHDAY MLADY MAHEEN!</h1>
      <div class="date">NOVEMBER 12, 2026</div>

      <div class="photo-frame">
        <div class="heart">♥</div>

        <div class="polaroid" aria-label="Silly birthday face">
          <svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Silly face">
            <rect width="200" height="200" fill="#f6f0f2"/>
            <g stroke="#151115" stroke-width="7" stroke-linecap="round" stroke-linejoin="round">
              <path d="M38 42c22-28 92-30 119 0 15 17 20 36 20 64 0 50-25 79-71 85-54 7-96-16-99-72-2-33 9-55 31-77Z" fill="#f8f8f8"/>
              <ellipse cx="75" cy="90" rx="20" ry="28" fill="#0e0e0e"/>
              <ellipse cx="126" cy="90" rx="20" ry="28" fill="#0e0e0e"/>
              <circle cx="82" cy="89" r="6" fill="#ffffff"/>
              <circle cx="133" cy="89" r="6" fill="#ffffff"/>
              <ellipse cx="82" cy="120" rx="12" ry="8" fill="#f5b2c0"/>
              <ellipse cx="118" cy="120" rx="12" ry="8" fill="#f5b2c0"/>
              <path d="M72 131c13 16 35 18 52 0" fill="none"/>
              <path d="M70 140c16 19 43 19 57 0" fill="none"/>
            </g>
          </svg>
        </div>

        <div class="polaroid" aria-label="Silly birthday face with roses">
          <svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Silly face with roses">
            <rect width="200" height="200" fill="#f8f1f3"/>
            <g stroke="#171217" stroke-width="7" stroke-linecap="round" stroke-linejoin="round">
              <path d="M36 44c22-22 88-28 119 2 18 18 22 40 22 72 0 47-27 75-72 80-58 7-95-20-98-73-2-36 9-57 29-81Z" fill="#f6f6f6"/>
              <ellipse cx="76" cy="90" rx="18" ry="27" fill="#0e0e0e"/>
              <ellipse cx="123" cy="90" rx="18" ry="27" fill="#0e0e0e"/>
              <circle cx="81" cy="89" r="6" fill="#ffffff"/>
              <circle cx="127" cy="89" r="6" fill="#ffffff"/>
              <ellipse cx="77" cy="119" rx="12" ry="8" fill="#f5b7c4"/>
              <ellipse cx="121" cy="119" rx="12" ry="8" fill="#f5b7c4"/>
              <path d="M63 129c12 14 33 18 52 0" fill="none"/>
              <path d="M62 138c15 17 44 18 60 0" fill="none"/>
            </g>

            <g transform="translate(108,118)">
              <g fill="#d51d3f" stroke="#440d1e" stroke-width="2">
                <circle cx="0" cy="0" r="10"/>
                <circle cx="-10" cy="10" r="10"/>
                <circle cx="10" cy="10" r="10"/>
                <circle cx="-16" cy="-4" r="10"/>
                <circle cx="16" cy="-4" r="10"/>
                <circle cx="-6" cy="-12" r="10"/>
                <circle cx="6" cy="-12" r="10"/>
              </g>
              <g stroke="#381b23" stroke-width="2">
                <path d="M0 8v45" fill="none"/>
                <path d="M-1 30c-6-5-10-12-10-20" fill="none"/>
                <path d="M1 30c6-5 10-12 10-20" fill="none"/>
              </g>
            </g>
          </svg>
        </div>
      </div>

      <p class="hint">A birthday letter is hiding in the tiny cake ♡</p>
    </section>

    <div class="cake-label">tap the cake!</div>
    <button class="cake-button" id="openLetter" aria-label="Open birthday letter">
      <span class="tiny-cake">
        <span class="cake-top"></span>
        <span class="candle"></span>
        <span class="flame"></span>
        <span class="cake-body"></span>
        <span class="cherry"></span>
      </span>
    </button>
  </main>

  <div class="overlay" id="overlay" aria-hidden="true">
    <div class="letter-box" role="dialog" aria-modal="true">
      <button class="close-btn" id="closeLetter" aria-label="Close birthday letter">×</button>
      <h2>HAPPY BIRTHDAY MLADY MAHEEN!</h2>
      <p>HAPPY BIRTHDAY MLADY MAHEEN! I LOVE U! LOOK AT U TURNING 13, MY LIL GURL TURNED 13 IM PROUD OF U SM I DAT I CANT EVEN TELL =D
Welcome to da teenage era :3 I LOVE U MLADY MAY ALLAH BLESS U AND ALWAYS KEEP U HAPPY AND HELP U SUCCESS IN EVERY, EVERY SINGLE THING, AMEEN! =D</p>
    </div>
  </div>

  <script>
    const stars = document.getElementById("stars");
    const colors = ["#fff", "#ffd7f0", "#d9d0ff", "#fff3b5", "#dff6ff"];

    for (let i = 0; i < 40; i++) {
      const s = document.createElement("span");
      s.className = "sparkle";
      s.textContent = Math.random() > 0.5 ? "✦" : "❄";
      s.style.setProperty("--x", `${Math.random() * 100}%`);
      s.style.setProperty("--s", `${10 + Math.random() * 12}px`);
      s.style.setProperty("--c", colors[Math.floor(Math.random() * colors.length)]);
      s.style.setProperty("--dur", `${7 + Math.random() * 8}s`);
      s.style.setProperty("--delay", `${-Math.random() * 12}s`);
      s.style.setProperty("--drift", `${Math.random() * 82 - 41}px`);
      stars.appendChild(s);
    }

    const overlay = document.getElementById("overlay");
    const openBtn = document.getElementById("openLetter");
    const closeBtn = document.getElementById("closeLetter");

    function openLetter() {
      overlay.classList.add("open");
      overlay.setAttribute("aria-hidden", "false");
      closeBtn.focus();
    }

    function closeLetter() {
      overlay.classList.remove("open");
      overlay.setAttribute("aria-hidden", "true");
      openBtn.focus();
    }

    openBtn.addEventListener("click", openLetter);
    closeBtn.addEventListener("click", closeLetter);

    overlay.addEventListener("click", (e) => {
      if (e.target === overlay) closeLetter();
    });

    document.addEventListener("keydown", (e) => {
      if (e.key === "Escape" && overlay.classList.contains("open")) {
        closeLetter();
      }
    });
  </script>
</body>
</html>
