---
layout: none
permalink: /personal/happy-bday-love/
---

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Happy Birthday, My Love</title>
    <style>
      :root {
        --deep-night: #120b1a;
        --blush: #ef7c8e;
        --pale-gold: #f4c095;
        --paper: #fffdf6;
        --ink: #3a2c2f;
        --lavender: #c6cffd;
      }

      * {
        box-sizing: border-box;
      }

      body {
        margin: 0;
        min-height: 100vh;
        font-family: "Playfair Display", "Poppins", "Segoe UI", system-ui, -apple-system, sans-serif;
        background: radial-gradient(circle at top, #ffe0ea 0%, #fef6f6 45%, #f8f2ff 100%);
        color: var(--ink);
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 2rem 1rem;
        position: relative;
        overflow-x: hidden;
      }

      body::before,
      body::after {
        content: "";
        position: fixed;
        inset: 0;
        pointer-events: none;
      }

      body::before {
        background: url('data:image/svg+xml,%3Csvg width="120" height="120" viewBox="0 0 120 120" xmlns="http://www.w3.org/2000/svg"%3E%3Cg fill="none" fill-opacity="0.13"%3E%3Cpath d="M60 13l4.08 12.54h13.18l-10.66 7.75 4.08 12.55L60 38.07l-10.68 7.77 4.08-12.55-10.66-7.75h13.18z" fill="%23ef7c8e"/%3E%3Cpath d="M16 83l2.72 8.33h8.7l-7.03 5.11 2.72 8.33L16 99.66l-7.1 5.11 2.72-8.33-7.03-5.11h8.7z" fill="%23f4c095"/%3E%3C/g%3E%3C/svg%3E')
          repeat center/180px 180px;
        opacity: 0.4;
      }

      body::after {
        background: radial-gradient(circle, rgba(255, 255, 255, 0) 40%, rgba(255, 255, 255, 0.6) 100%);
      }

      main {
        width: min(96vw, 980px);
        min-height: min(85vh, 640px);
        display: flex;
        align-items: center;
        justify-content: center;
        position: relative;
        z-index: 1;
      }

      .scene {
        width: 100%;
        height: 100%;
        perspective: 2000px;
        display: flex;
        align-items: center;
        justify-content: center;
      }

      .diary {
        width: min(90vw, 820px);
        min-height: min(75vh, 560px);
        position: relative;
        transform-style: preserve-3d;
        transition: transform 1.2s ease;
      }

      .cover,
      .page {
        position: absolute;
        inset: 0;
        border-radius: 28px;
      }

      .cover {
        transform-origin: left center;
        background: linear-gradient(135deg, #2d233b, #4b3d60 60%, #8f769c);
        box-shadow: 0 30px 50px rgba(18, 11, 26, 0.4);
        border: 2px solid rgba(255, 255, 255, 0.15);
        color: #fff;
        padding: 3rem;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: center;
        gap: 1rem;
        letter-spacing: 0.08em;
        text-transform: uppercase;
        font-weight: 600;
        transform: rotateY(0deg);
        transition: transform 1.2s ease, box-shadow 1.2s ease;
        z-index: 3;
      }

      .cover h1 {
        margin: 0;
        font-size: clamp(1.2rem, 2vw, 1.8rem);
        letter-spacing: 0.3em;
      }

      .cover span.lock {
        font-size: 2.4rem;
      }

      .cover p {
        margin: 0;
        font-size: 0.95rem;
        text-transform: none;
        opacity: 0.8;
        max-width: 320px;
      }

      .diary.open .cover {
        transform: rotateY(-165deg);
        box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
      }

      .page {
        background: var(--paper);
        background-image: repeating-linear-gradient(
            transparent,
            transparent 34px,
            rgba(0, 0, 0, 0.04) 34px,
            rgba(0, 0, 0, 0.04) 35px
          ),
          linear-gradient(120deg, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0.2));
        padding: clamp(1.4rem, 2vw, 3rem);
        box-shadow: 0 30px 50px rgba(18, 11, 26, 0.25);
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        position: relative;
        overflow: hidden;
        z-index: 1;
      }

      .page::before {
        content: "";
        position: absolute;
        left: clamp(1.4rem, 2.5vw, 3.4rem);
        top: 0;
        bottom: 0;
        width: 0.18rem;
        background: linear-gradient(180deg, rgba(0, 0, 0, 0.05), rgba(0, 0, 0, 0.2));
        box-shadow: 0 0 15px rgba(0, 0, 0, 0.2);
        opacity: 0.4;
      }

      .video-wrapper {
        width: min(100%, 620px);
        background: rgba(255, 255, 255, 0.85);
        border-radius: 22px;
        padding: clamp(1rem, 2vw, 1.6rem);
        position: relative;
        box-shadow: 0 20px 40px rgba(31, 25, 43, 0.15);
        border: 1px solid rgba(15, 7, 19, 0.05);
      }

      .video-wrapper::before,
      .video-wrapper::after {
        content: "";
        position: absolute;
        width: 70px;
        height: 18px;
        background: rgba(255, 255, 255, 0.6);
        border-radius: 6px;
        top: 12px;
        box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1);
      }

      .video-wrapper::before {
        left: 50px;
        transform: rotate(-6deg);
      }

      .video-wrapper::after {
        right: 50px;
        transform: rotate(8deg);
      }

      .video-title {
        font-family: "Playfair Display", serif;
        font-size: 1.1rem;
        margin: 0 0 0.8rem;
        color: rgba(26, 10, 26, 0.7);
        text-align: center;
        letter-spacing: 0.06em;
      }

      video {
        width: 100%;
        height: auto;
        max-height: min(65vh, 420px);
        border-radius: 18px;
        background: #02040a;
        display: block;
        box-shadow: inset 0 0 0 2px rgba(255, 255, 255, 0.35);
      }

      .custom-controls {
        margin-top: 1rem;
        display: flex;
        align-items: center;
        gap: 0.7rem;
        flex-wrap: wrap;
        background: rgba(255, 255, 255, 0.9);
        padding: 0.75rem 1.1rem;
        border-radius: 999px;
        box-shadow: 0 6px 14px rgba(18, 11, 26, 0.15);
      }

      .custom-controls button {
        border: none;
        background: linear-gradient(135deg, var(--blush), #fbb1bd);
        color: #fff;
        font-weight: 600;
        letter-spacing: 0.04em;
        padding: 0.4rem 0.95rem;
        border-radius: 999px;
        cursor: pointer;
        transition: transform 0.2s ease, box-shadow 0.2s ease;
        font-size: 0.85rem;
      }

      .custom-controls button:hover {
        transform: translateY(-1px);
        box-shadow: 0 8px 14px rgba(239, 124, 142, 0.35);
      }

      .time-display {
        font-size: 0.85rem;
        color: rgba(15, 7, 19, 0.65);
        min-width: 90px;
        text-align: center;
        font-variant-numeric: tabular-nums;
      }

      .progress {
        flex: 1;
        -webkit-appearance: none;
        appearance: none;
        height: 6px;
        border-radius: 999px;
        background: rgba(130, 96, 122, 0.3);
        outline: none;
        cursor: pointer;
      }

      .progress::-webkit-slider-thumb {
        -webkit-appearance: none;
        width: 16px;
        height: 16px;
        border-radius: 50%;
        background: var(--blush);
        box-shadow: 0 0 0 3px rgba(239, 124, 142, 0.25);
        border: 1px solid #fff;
      }

      .progress::-moz-range-thumb {
        width: 16px;
        height: 16px;
        border-radius: 50%;
        background: var(--blush);
        border: 2px solid #fff;
        box-shadow: 0 0 0 3px rgba(239, 124, 142, 0.25);
      }

      .note {
        margin-top: 1.3rem;
        font-style: italic;
        text-align: center;
        color: rgba(35, 20, 40, 0.7);
        letter-spacing: 0.03em;
      }

      .password-overlay {
        position: fixed;
        inset: 0;
        background: rgba(9, 5, 15, 0.85);
        backdrop-filter: blur(8px);
        display: flex;
        align-items: center;
        justify-content: center;
        z-index: 10;
        transition: opacity 0.45s ease;
      }

      .password-overlay.hidden {
        opacity: 0;
        visibility: hidden;
        pointer-events: none;
      }

      .password-overlay.shake .password-card {
        animation: shake 0.4s ease;
      }

      .password-card {
        background: linear-gradient(160deg, #24182f, #402248 60%, #633661);
        border-radius: 24px;
        padding: 2.2rem;
        color: #fff;
        width: min(90vw, 370px);
        text-align: center;
        box-shadow: 0 30px 60px rgba(0, 0, 0, 0.5);
        border: 1px solid rgba(255, 255, 255, 0.15);
        animation: float 4s ease-in-out infinite;
      }

      .password-card h2 {
        margin: 0 0 0.5rem;
        letter-spacing: 0.1em;
        text-transform: uppercase;
      }

      .password-card p {
        margin: 0 0 1.6rem;
        opacity: 0.8;
      }

      .password-input {
        display: flex;
        gap: 0.6rem;
        margin-bottom: 0.8rem;
      }

      .password-input input {
        flex: 1;
        border-radius: 999px;
        border: 1px solid rgba(255, 255, 255, 0.4);
        padding: 0.5rem 1rem;
        font-size: 1rem;
        background: rgba(255, 255, 255, 0.1);
        color: #fff;
      }

      .password-input input::placeholder {
        color: rgba(255, 255, 255, 0.6);
      }

      .password-input button {
        border: none;
        border-radius: 999px;
        padding: 0 1.2rem;
        background: linear-gradient(130deg, var(--blush), var(--pale-gold));
        color: #140c1d;
        font-weight: 700;
        text-transform: uppercase;
        letter-spacing: 0.08em;
        cursor: pointer;
        transition: transform 0.2s ease;
      }

      .password-input button:hover {
        transform: translateY(-1px);
      }

      .password-card small {
        display: block;
        opacity: 0.7;
        letter-spacing: 0.05em;
      }

      .birthday-message {
        position: fixed;
        left: 50%;
        bottom: -20%;
        transform: translate(-50%, 0);
        background: rgba(255, 255, 255, 0.88);
        color: var(--deep-night);
        padding: 1.2rem 2.4rem;
        border-radius: 999px;
        font-size: clamp(1.3rem, 4vw, 2.4rem);
        font-family: "Playfair Display", serif;
        letter-spacing: 0.08em;
        text-transform: uppercase;
        box-shadow: 0 25px 45px rgba(0, 0, 0, 0.2);
        opacity: 0;
        transition: transform 0.8s ease, opacity 0.8s ease;
        z-index: 5;
        pointer-events: none;
      }

      .birthday-message.show {
        bottom: 50%;
        transform: translate(-50%, 50%);
        opacity: 1;
        pointer-events: auto;
      }

      .confetti-canvas {
        position: fixed;
        inset: 0;
        width: 100vw;
        height: 100vh;
        pointer-events: none;
        z-index: 4;
        opacity: 0;
        transition: opacity 0.3s ease;
      }

      .confetti-canvas.show {
        opacity: 1;
      }

      @keyframes float {
        0%,
        100% {
          transform: translateY(0);
        }
        50% {
          transform: translateY(-7px);
        }
      }

      @keyframes shake {
        10%,
        90% {
          transform: translate3d(-1px, 0, 0);
        }
        20%,
        80% {
          transform: translate3d(2px, 0, 0);
        }
        30%,
        50%,
        70% {
          transform: translate3d(-4px, 0, 0);
        }
        40%,
        60% {
          transform: translate3d(4px, 0, 0);
        }
      }

      @media (max-width: 768px) {
        body {
          padding: 1.5rem 0.8rem;
          align-items: flex-start;
        }

        main {
          width: 100%;
          min-height: auto;
        }

        .diary {
          width: 100%;
          min-height: 520px;
        }

        .cover {
          padding: 2rem;
        }

        .page {
          padding: 1.2rem 1rem 2rem;
        }

        .video-wrapper {
          padding: 1rem;
        }

        .custom-controls {
          border-radius: 22px;
        }

        .birthday-message {
          width: 90%;
          text-align: center;
        }

        video {
          max-height: 45vh;
        }
      }

      @media (max-width: 600px) {
        .custom-controls {
          flex-direction: column;
          align-items: stretch;
          gap: 0.5rem;
        }

        .time-display,
        .progress,
        .custom-controls button {
          width: 100%;
          text-align: center;
        }

        .time-display {
          order: -1;
        }
      }
    </style>
  </head>
  <body>
    <div class="password-overlay" id="passwordOverlay">
      <div class="password-card">
        <h2>dear diary</h2>
        <p>
          Whisper the little password we share and
          I will open up to you.
        </p>
        <div class="password-input">
          <input
            id="passwordInput"
            type="password"
            placeholder="Our secret word"
            autocomplete="off"
            aria-label="Password"
          />
          <button id="unlockButton" aria-label="Unlock diary">Open</button>
        </div>
        <small id="passwordHint">She is cute, fluffy, and my best investment till now! </small>
      </div>
    </div>

    <main>
      <div class="scene">
        <div class="diary" id="diary">
          <div class="cover">
            <span class="lock">🔒</span>
            <h1>OUR LITTLE DIARY</h1>
            <p>Turn the page with the word that only your heart remembers.</p>
          </div>
          <div class="page">
            <div class="video-wrapper">
              <p class="video-title"></p>
              <video
                id="loveVideo"
                playsinline
                webkit-playsinline
                preload="metadata"
                disablepictureinpicture
                controlslist="nodownload noremoteplayback"
              ></video>
              <div class="custom-controls">
                <button id="playPause" aria-label="Play or pause video">Play</button>
                <div class="time-display">
                  <span id="currentTime">0:00</span> / <span id="duration">0:00</span>
                </div>
                <input
                  id="progress"
                  class="progress"
                  type="range"
                  min="0"
                  max="100"
                  value="0"
                  step="0.1"
                  aria-label="Seek"
                />
                <button id="muteToggle" aria-label="Mute or unmute">Mute</button>
              </div>
              <p class="note">
                Relax, take a deep breath, and let these seconds remind you that I admire you for all that you are, and that you should be proud of yourself for everything you’ve accomplished.
              </p>
            </div>
          </div>
        </div>
      </div>
    </main>

    <div class="birthday-message">Happy birthday my love ❤️</div>
    <canvas id="confettiCanvas" class="confetti-canvas" aria-hidden="true"></canvas>

    <script>
      (() => {
        const PASSWORD = "hedwig"; // Change to any word you both know.
        const VIDEO_URL = "https://rudresh.net/assets/video/abhi_tu_meri_bhi_kahani.mp4"; // Replace with your hosted video link if needed.

        const overlay = document.getElementById("passwordOverlay");
        const diary = document.getElementById("diary");
        const passwordInput = document.getElementById("passwordInput");
        const unlockButton = document.getElementById("unlockButton");
        const hint = document.getElementById("passwordHint");
        const video = document.getElementById("loveVideo");
        const playPause = document.getElementById("playPause");
        const muteToggle = document.getElementById("muteToggle");
        const progress = document.getElementById("progress");
        const currentTimeEl = document.getElementById("currentTime");
        const durationEl = document.getElementById("duration");
        const message = document.querySelector(".birthday-message");
        const confettiCanvas = document.getElementById("confettiCanvas");
        const confettiCtx = confettiCanvas.getContext("2d");
        const prefersReducedMotion = window.matchMedia("(prefers-reduced-motion: reduce)");
        let confettiAnimation;
        let messageTimeoutId;

        const outsideClickHandler = (event) => {
          if (!message.contains(event.target)) {
            hideBirthdayMessage();
          }
        };

        video.src = VIDEO_URL;

        function resizeConfettiCanvas() {
          if (!confettiCanvas) {
            return;
          }
          confettiCanvas.width = window.innerWidth;
          confettiCanvas.height = window.innerHeight;
        }

        resizeConfettiCanvas();
        window.addEventListener("resize", resizeConfettiCanvas);

        function unlockDiary() {
          const attempt = passwordInput.value.trim().toLowerCase();
          if (!attempt) {
            return;
          }

          if (attempt === PASSWORD.toLowerCase()) {
            overlay.classList.add("hidden");
            setTimeout(() => {
              diary.classList.add("open");
              video.focus();
            }, 200);
          } else {
            overlay.classList.add("shake");
            hint.textContent = "psst... try the nickname you whisper to me.";
            setTimeout(() => overlay.classList.remove("shake"), 480);
          }
        }

        unlockButton.addEventListener("click", (event) => {
          event.preventDefault();
          unlockDiary();
        });

        passwordInput.addEventListener("keydown", (event) => {
          if (event.key === "Enter") {
            event.preventDefault();
            unlockDiary();
          }
        });

        function formatTime(seconds) {
          const mins = Math.floor(seconds / 60) || 0;
          const secs = Math.floor(seconds % 60) || 0;
          return `${mins}:${secs.toString().padStart(2, "0")}`;
        }

        video.addEventListener("loadedmetadata", () => {
          durationEl.textContent = formatTime(video.duration);
        });

        video.addEventListener("timeupdate", () => {
          if (!Number.isFinite(video.duration)) {
            return;
          }
          const percent = (video.currentTime / video.duration) * 100;
          progress.value = percent;
          currentTimeEl.textContent = formatTime(video.currentTime);
        });

        progress.addEventListener("input", () => {
          if (!Number.isFinite(video.duration)) {
            return;
          }
          const seekTime = (progress.value / 100) * video.duration;
          video.currentTime = seekTime;
        });

        playPause.addEventListener("click", () => {
          if (video.paused) {
            video.play();
          } else {
            video.pause();
          }
        });

        video.addEventListener("play", () => {
          playPause.textContent = "Pause";
        });

        video.addEventListener("pause", () => {
          playPause.textContent = video.ended ? "Replay" : "Play";
        });

        muteToggle.addEventListener("click", () => {
          video.muted = !video.muted;
          muteToggle.textContent = video.muted ? "Unmute" : "Mute";
        });

        video.addEventListener("ended", () => {
          launchConfetti();
          showBirthdayMessage();
        });

        function showBirthdayMessage() {
          message.classList.add("show");
          clearTimeout(messageTimeoutId);
          messageTimeoutId = setTimeout(hideBirthdayMessage, 5000);
          document.addEventListener("pointerdown", outsideClickHandler);
        }

        function hideBirthdayMessage() {
          if (!message.classList.contains("show")) {
            return;
          }
          message.classList.remove("show");
          clearTimeout(messageTimeoutId);
          document.removeEventListener("pointerdown", outsideClickHandler);
        }

        function launchConfetti() {
          if (!confettiCanvas || prefersReducedMotion.matches) {
            return;
          }

          cancelAnimationFrame(confettiAnimation);
          confettiCanvas.classList.add("show");

          const colors = ["#ef7c8e", "#5f6caf", "#ffd3b6", "#f4c095", "#9ad5ca", "#f7aef8"];
          const pieces = Array.from({ length: 190 }, () => ({
            x: Math.random() * confettiCanvas.width,
            y: Math.random() * -confettiCanvas.height,
            size: 6 + Math.random() * 6,
            speed: 2 + Math.random() * 3,
            drift: -1.5 + Math.random() * 3,
            rotation: Math.random() * 360,
            rotationSpeed: -3 + Math.random() * 6,
            color: colors[Math.floor(Math.random() * colors.length)],
            opacity: 0.7 + Math.random() * 0.3,
          }));
          const endTime = performance.now() + 5000;

          function draw(now) {
            confettiCtx.clearRect(0, 0, confettiCanvas.width, confettiCanvas.height);

            pieces.forEach((piece) => {
              piece.y += piece.speed;
              piece.x += piece.drift;
              piece.rotation += piece.rotationSpeed;

              if (piece.y > confettiCanvas.height) {
                piece.y = -10;
                piece.x = Math.random() * confettiCanvas.width;
              }

              if (piece.x > confettiCanvas.width) {
                piece.x = 0;
              } else if (piece.x < 0) {
                piece.x = confettiCanvas.width;
              }

              confettiCtx.save();
              confettiCtx.globalAlpha = piece.opacity;
              confettiCtx.translate(piece.x, piece.y);
              confettiCtx.rotate((piece.rotation * Math.PI) / 180);
              confettiCtx.fillStyle = piece.color;
              confettiCtx.fillRect(-piece.size / 2, -piece.size / 2, piece.size, piece.size * 0.45);
              confettiCtx.restore();
            });

            if (now < endTime) {
              confettiAnimation = requestAnimationFrame(draw);
            } else {
              confettiCanvas.classList.remove("show");
              confettiCtx.clearRect(0, 0, confettiCanvas.width, confettiCanvas.height);
            }
          }

          confettiAnimation = requestAnimationFrame(draw);
        }
      })();
    </script>
  </body>
</html>
