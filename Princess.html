<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Lil Cookie's Birthday</title>
<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --beige: #f1e6cf;
    --pink: #f4b8c4;
    --brown: #7a3e3e;
    --paper: #f8e1e1;
    --ink: #1c1412;
  }

  html, body { height: 100%; }
  body { font-family: "Times New Roman", serif; color: var(--ink); overflow: hidden; }

  /* ---------- pages ---------- */
  .page {
    position: absolute; inset: 0;
    display: none;
    flex-direction: column; align-items: center; justify-content: center;
    padding: 24px; text-align: center; overflow: hidden;
  }
  .page.active { display: flex; }
  #page1 { background: var(--beige); }
  #page2 { background: var(--pink); }
  #page3 { background: #fff3d6; }

  h1 { font-size: clamp(2rem, 8vw, 3.5rem); margin-bottom: 36px; position: relative; z-index: 2; }

  /* ---------- retro 3D buttons ---------- */
  .btn {
    font: bold 1.2rem "Times New Roman", serif;
    padding: 16px 40px;
    background: #f5f5f5; color: var(--ink);
    border: 2px solid var(--ink); border-radius: 5px;
    box-shadow: 0 8px 0 #777, 0 12px 20px rgba(0,0,0,.3);
    cursor: pointer; position: relative; z-index: 2;
    transition: transform .15s, box-shadow .15s;
  }
  .btn:active { transform: translateY(8px); box-shadow: 0 0 0 #777, 0 4px 8px rgba(0,0,0,.3); }
  .btn:focus-visible, .closeButton:focus-visible { outline: 3px solid var(--brown); outline-offset: 3px; }

  /* ---------- page 1: glow + falling flowers ---------- */
  #page1::before, #page1::after {
    content: ""; position: absolute; width: 110px; height: 110px; border-radius: 50%;
    background: rgba(255, 220, 100, .8); filter: blur(25px);
    animation: glow 2s infinite alternate;
  }
  #page1::before { top: 20px; left: 20px; }
  #page1::after  { bottom: 20px; right: 20px; }
  @keyframes glow { from { opacity: .4; transform: scale(.9); } to { opacity: 1; transform: scale(1.2); } }

  .flower { position: absolute; top: -50px; font-size: 26px; pointer-events: none; animation: fall linear forwards; }
  @keyframes fall { to { transform: translateY(115vh) rotate(360deg); } }

  /* ---------- page 2: popup ---------- */
  .popup {
    position: relative; width: min(320px, 90vw); min-height: 150px; padding: 20px;
    background: var(--paper); border: 3px solid var(--brown); border-radius: 8px;
    display: flex; align-items: center; justify-content: center;
    box-shadow: 8px 8px 0 #8b5a5a, 12px 12px 20px rgba(0,0,0,.3);
    animation: floatingPopup 3s ease-in-out infinite;
  }
  .popup p { font-size: 1.3rem; font-weight: bold; color: var(--brown); }
  @keyframes floatingPopup { 0%, 100% { transform: translateX(-20px); } 50% { transform: translateX(20px); } }

  .closeButton {
    position: absolute; top: 8px; right: 8px; width: 30px; height: 30px;
    background: #fff; border: 2px solid var(--brown); box-shadow: 3px 3px 0 var(--brown);
    font: bold 20px "Times New Roman", serif; cursor: pointer;
  }

  .buttons { margin-top: 50px; display: flex; flex-direction: column; gap: 20px; align-items: center; }
  .buttons .btn { width: 170px; padding: 12px 0; font-size: 1rem; box-shadow: 5px 5px 0 #555; }
  .buttons .btn:active { transform: translate(5px, 5px); box-shadow: 0 0 0 #555; }
  #denyButton { transition: left .25s, top .25s, transform .15s, box-shadow .15s; }
  #denyButton.runaway { position: fixed; }

  /* ---------- page 3: celebration ---------- */
  .cake { font-size: clamp(4rem, 18vw, 7rem); animation: bounce 1.2s ease-in-out infinite; }
  @keyframes bounce { 50% { transform: translateY(-14px); } }
  #page3 h1 { margin: 10px 0 16px; color: var(--brown); }
  .message { max-width: 34ch; font-size: 1.25rem; line-height: 1.6; }

  .confetti { position: absolute; top: -20px; width: 10px; height: 16px; animation: fall linear forwards; pointer-events: none; }

  /* ---------- page 4: catch the cookies ---------- */
  #page4 { background: #d9ecf2; justify-content: flex-start; touch-action: manipulation; user-select: none; }
  .hud { position: relative; z-index: 3; display: flex; gap: 32px; font-size: 1.5rem; font-weight: bold; color: var(--brown); margin-top: 8px; }
  .item { position: absolute; top: -60px; font-size: 44px; cursor: pointer; animation: fall linear forwards; }
  .item.pop { animation: pop .25s ease-out forwards; }
  @keyframes pop { to { transform: scale(1.8); opacity: 0; } }
  #gameResult { position: absolute; inset: 0; z-index: 4; display: none; flex-direction: column; align-items: center; justify-content: center; gap: 18px; background: rgba(255,243,214,.94); padding: 24px; }
  #gameResult.show { display: flex; }
  #gameResult h2 { font-size: clamp(1.8rem, 7vw, 2.6rem); color: var(--brown); }
  #gameResult p { font-size: 1.2rem; max-width: 30ch; }
  .row { display: flex; gap: 16px; flex-wrap: wrap; justify-content: center; }
  #page3 .btn { margin-top: 28px; }

  @media (prefers-reduced-motion: reduce) {
    .popup, .cake, #page1::before, #page1::after { animation: none; }
  }
</style>
</head>
<body>

<!-- PAGE 1 -->
<section id="page1" class="page active">
  <h1>Lil Cookie's Birthday</h1>
  <button id="surpriseButton" class="btn">SURPRISE</button>
</section>

<!-- PAGE 2 -->
<section id="page2" class="page">
  <div class="popup">
    <button class="closeButton" id="closeButton" aria-label="Close">×</button>
    <p>You are my cutie</p>
  </div>
  <div class="buttons">
    <button id="acceptButton" class="btn">ACCEPT</button>
    <button id="denyButton" class="btn">DENY</button>
  </div>
</section>

<!-- PAGE 3 -->
<section id="page3" class="page">
  <div class="cake">🎂</div>
  <h1>Happy Birthday!</h1>
  <p class="message">PALAK (LIL COOKIE)!🫶 You're genuinely one of the solus I Know🥹. May your Day be as Special, beautiful & adorable as you are🌸💗.</p>
  <button id="playButton" class="btn">PLAY A GAME</button>
</section>

<!-- PAGE 4: GAME -->
<section id="page4" class="page">
  <div class="hud"><span>Score: <span id="score">0</span></span><span>Time: <span id="time">20</span></span></div>
  <div id="gameResult">
    <h2>Time's up!</h2>
    <p id="resultText"></p>
    <div class="row">
      <button id="againButton" class="btn">PLAY AGAIN</button>
      <button id="backButton" class="btn">BACK</button>
    </div>
  </div>
</section>

<script>
  const $ = (id) => document.getElementById(id);

  function showPage(pageId) {
    document.querySelectorAll(".page").forEach(p => p.classList.remove("active"));
    $(pageId).classList.add("active");
  }

  /* falling flowers: only while page 1 is visible */
  const flowers = ["🌸", "🌷", "🌺", "🌼", "💮"];
  setInterval(() => {
    if (!$("page1").classList.contains("active")) return;
    const f = document.createElement("div");
    f.className = "flower";
    f.textContent = flowers[Math.floor(Math.random() * flowers.length)];
    f.style.left = Math.random() * 100 + "vw";
    f.style.animationDuration = (4 + Math.random() * 5) + "s";
    $("page1").appendChild(f);
    setTimeout(() => f.remove(), 9000);
  }, 500);

  /* navigation */
  $("surpriseButton").addEventListener("click", () => showPage("page2"));
  $("closeButton").addEventListener("click", () => {
    $("closeButton").parentElement.style.transform = "scale(1.05)"; // popup refuses to close
    setTimeout(() => $("closeButton").parentElement.style.transform = "", 200);
  });

  /* DENY runs away from cursor/finger */
  const deny = $("denyButton");
  function dodge() {
    const pad = 20;
    const maxX = window.innerWidth  - deny.offsetWidth  - pad;
    const maxY = window.innerHeight - deny.offsetHeight - pad;
    deny.classList.add("runaway");
    deny.style.left = pad + Math.random() * (maxX - pad) + "px";
    deny.style.top  = pad + Math.random() * (maxY - pad) + "px";
  }
  deny.addEventListener("mouseenter", dodge);
  deny.addEventListener("touchstart", (e) => { e.preventDefault(); dodge(); }, { passive: false });
  deny.addEventListener("click", dodge); // keyboard users get the same joke

  /* ---------- game: catch the cookies ---------- */
  const GAME_SECONDS = 20;
  let score = 0, timeLeft = 0, tick = null, spawner = null, playing = false;

  function spawnItem() {
    if (!playing) return;
    const bonus = Math.random() < 0.12;          // cake = 5 points
    const el = document.createElement("div");
    el.className = "item";
    el.textContent = bonus ? "🎂" : "🍪";
    el.style.left = 4 + Math.random() * 82 + "vw";
    el.style.animationDuration = (2.2 + Math.random() * 1.8) + "s";
    el.addEventListener("pointerdown", () => {
      if (!playing || el.classList.contains("pop")) return;
      score += bonus ? 5 : 1;
      $("score").textContent = score;
      el.classList.add("pop");
      setTimeout(() => el.remove(), 250);
    });
    el.addEventListener("animationend", () => el.remove());
    $("page4").appendChild(el);
    // gets faster as time runs out
    const delay = 250 + (timeLeft / GAME_SECONDS) * 550;
    spawner = setTimeout(spawnItem, delay);
  }

  function startGame() {
    score = 0; timeLeft = GAME_SECONDS; playing = true;
    $("score").textContent = 0; $("time").textContent = timeLeft;
    $("gameResult").classList.remove("show");
    document.querySelectorAll(".item").forEach(i => i.remove());
    showPage("page4");
    spawnItem();
    tick = setInterval(() => {
      timeLeft--;
      $("time").textContent = timeLeft;
      if (timeLeft <= 0) endGame();
    }, 1000);
  }

  function endGame() {
    playing = false;
    clearInterval(tick); clearTimeout(spawner);
    const best = Math.max(score, Number(sessionStorage.getItem("best") || 0));
    sessionStorage.setItem("best", best);
    $("resultText").textContent = "You caught " + score + " points. Best this visit: " + best + ".";
    $("gameResult").classList.add("show");
  }

  $("playButton").addEventListener("click", startGame);
  $("againButton").addEventListener("click", startGame);
  $("backButton").addEventListener("click", () => showPage("page3"));

  /* ACCEPT -> celebration with confetti */
  $("acceptButton").addEventListener("click", () => {
    showPage("page3");
    const colors = ["#f4b8c4", "#f7c948", "#7a3e3e", "#8ecae6", "#b5e48c"];
    for (let i = 0; i < 80; i++) {
      const c = document.createElement("div");
      c.className = "confetti";
      c.style.left = Math.random() * 100 + "vw";
      c.style.background = colors[i % colors.length];
      c.style.animationDuration = (2 + Math.random() * 3) + "s";
      c.style.animationDelay = Math.random() * 1.5 + "s";
      $("page3").appendChild(c);
      setTimeout(() => c.remove(), 6000);
    }
  });
</script>
</body>
</html>
