---
title: about
layout: about
date: 2024-11-03 18:43:20
---

<style>
  /* ---------- Chips ---------- */
  .colorful-box {
    padding: 12px !important;
    border-radius: 10px;
    display: inline-block;
    color: white;
    font-weight: bold;
  }
  /* research: muted green */
  .generative-ai          { background-color: hsl(150, 28%, 40%); }
  .multimodal-dl          { background-color: hsl(138, 28%, 42%); }
  .large-language-models  { background-color: hsl(124, 27%, 44%); }
  .computer-vision        { background-color: hsl(100, 28%, 44%); }
  /* hobbies: muted blue */
  .music      { background-color: hsl(215, 34%, 48%); }
  .videogames { background-color: hsl(208, 36%, 48%); }
  .travelling { background-color: hsl(199, 38%, 46%); }
  .learning   { background-color: hsl(190, 38%, 44%); }
  /* selected pubs: warm, toned down to match */
  .pub1 { background-color: hsl(2, 42%, 52%); }
  .pub2 { background-color: hsl(23, 50%, 54%); }
  .pub3 { background-color: hsl(36, 52%, 52%); }
  /* ---------- Layout helpers ---------- */
  .center { text-align: center; }
  .chip-row {
    display: flex;
    justify-content: center;
    gap: 10px;
    flex-wrap: wrap;
    margin-top: 10px;
  }
  /* Research Interests + Hobbies: two equal-height cards */
  .info-cards {
    display: flex;
    align-items: stretch;
    gap: 20px;
    flex-wrap: wrap;
    margin: 1.5em 0;
  }
  .info-card {
    flex: 1 1 320px;
    box-sizing: border-box;
    padding: 10px;
    text-align: center;
    border: 1px solid rgba(128, 128, 128, 0.35);
    border-radius: 20px;
    background: rgba(128, 128, 128, 0.07);
    box-shadow: 0 4px 14px rgba(0, 0, 0, 0.08);
  }
  .info-card h2 {
    margin: 0 0 0.3em;
    padding: 0;
    border: none;
    font-size: 1.4em;
  }
  .info-card p { margin: 0 0 1em; opacity: 0.8; }
  .tag-row {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 12px;
  }
  @media (max-width: 420px) {
    .tag-row { grid-template-columns: 1fr; }
  }
  .tag {
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 10px 16px;
    border-radius: 20px;
    border: 2px solid rgba(255, 255, 255, 0.5);
    box-shadow: 0 3px 8px rgba(0, 0, 0, 0.2);
    font-size: 0.95em;
    transition: transform 0.15s ease;
  }
  .tag:hover { transform: translateY(-2px); }
  /* ---------- Contact links ---------- */
  .contact-row {
    display: flex;
    justify-content: center;
    gap: 14px;
    flex-wrap: wrap;
    margin: 1em 0;
  }
  .contact-row a { font-weight: bold; text-decoration: none; }
  /* ---------- Selected publications ---------- */
  .pub-row {
    display: flex;
    justify-content: center;
    align-items: stretch;
    gap: 10px;
    flex-wrap: wrap;
  }
  .pub-chip {
    position: relative;
    flex: 1 1 220px;
    max-width: 320px;
    box-sizing: border-box;
    padding: 14px 16px;
    text-align: center;
    border: 3px solid rgba(255, 255, 255, 0.55);
    border-radius: 20px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.25);
    transition: transform 0.15s ease, box-shadow 0.15s ease;
  }
  .pub-chip:hover {
    transform: translateY(-3px);
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
  }
  /* link inside the chip: forced to look like plain white text, and
     stretched so the whole chip is clickable */
  .pub-chip a {
    color: white !important;
    text-decoration: none !important;
    background: none !important;
    border: none !important;
    box-shadow: none !important;
  }
  .pub-chip a::after {
    content: "";
    position: absolute;
    inset: 0;
    border-radius: 18px;
  }
  .pub-chip .venue {
    display: block;
    margin-top: 8px;
    padding-top: 8px;
    border-top: 1px solid rgba(255, 255, 255, 0.4);
    font-size: 0.85em;
    font-weight: normal;
  }
  /* ---------- News ---------- */
  #news { padding-left: 1.2em; }
  #news li { margin-bottom: 0.8em; }
  .news-btn {
    display: none; /* shown by the script only when needed */
    margin: 10px auto 0;
    padding: 8px 20px;
    border: none;
    border-radius: 10px;
    background-color: #2274A5;
    color: white;
    font-weight: bold;
    cursor: pointer;
  }
  .news-btn:hover { opacity: 0.85; }
  .koi { max-width: 100%; height: auto; display: block; margin: 0 auto; }
  .info-card:nth-child(1) { border-top: 4px solid #357a45; }
  .info-card:nth-child(2) { border-top: 4px solid #1f64a3; }
  .pub-chip { border-color: rgba(255, 255, 255, 0.55); } /* unchanged, just to be explicit */
</style>

<div style="text-align:center;">

Hello there! I’m Ivan Rinaldi, a **PhD student** at the University of Bari Aldo Moro, based in Bari (BA), Apulia, Italy 🇮🇹, and currently a visiting researcher in Amiens, France 🇫🇷. I am working in the [CILab](https://cilab.di.uniba.it/) laboratory, pursuing a PhD on **"Advanced Generative Models for Conversion between Images, Text, and Audio"**, co-funded by [AIVB](https://aivb.ai/en/home/).

In July 2024, I earned my **Master's degree** in Computer Science (AI curriculum) at the [University of Bari Aldo Moro](https://www.uniba.it/en). My thesis focused on **Generative AI**, specifically diffusion models and conditioned music generation from artworks.

<!--  -->
<div class="info-cards">
  <div class="info-card">
    <h2>Research Interests 🔍</h2>
    <p>The topics I spend most of my research time on.</p>
    <div class="tag-row">
      <span class="colorful-box tag generative-ai">Generative AI 🌌</span>
      <span class="colorful-box tag multimodal-dl">Multimodal Deep Learning 🧩</span>
      <span class="colorful-box tag large-language-models">Large Language Models 🗣️</span>
      <span class="colorful-box tag computer-vision">Computer Vision 👁️</span>
    </div>
  </div>
  <div class="info-card">
    <h2>Hobbies 🕹️</h2>
    <p>When I’m not researching, I’m probably doing one of these.</p>
    <div class="tag-row">
      <span class="colorful-box tag music">Music 🎸</span>
      <span class="colorful-box tag videogames">Gaming 🎮</span>
      <span class="colorful-box tag travelling">Travelling ✈️</span>
      <span class="colorful-box tag learning">Learning new stuff 📚</span>
    </div>
  </div>
</div>
<!--  -->

<h1 class="center">Selected Publications 📖</h1>
 
<div class="pub-row">
  <div class="colorful-box pub1 pub-chip">
    <a href="https://dl.acm.org/doi/10.1145/3640457.3688137">Instructing and Prompting LLMs for Explainable Cross-domain Recommendations 🗣️</a>
    <span class="venue">RecSys 2024</span>
  </div>
  <div class="colorful-box pub2 pub-chip">
    <a href="https://link.springer.com/chapter/10.1007/978-3-031-92808-6_11">Art2Mus: Bridging Visual Arts and Music through Cross-Modal Generation 🎨🎹</a>
    <span class="venue">AI4VA@ECCV 2024 · Springer 2025</span>
  </div>
  <div class="colorful-box pub3 pub-chip">
    <a href="https://doi.org/10.1016/j.cviu.2026.104674">Handscribe: A Gloss-Free Framework for Sign Language Translation and Gloss Sequence Generation 🖐🏻</a>
    <span class="venue">CVIU Journal · 2026</span>
  </div>
</div>

# The Latest from Me

</div>

<div id="news">

- **October 2026**: Our work on audio analysis has been accepted for publication in the [**Multimedia Tools and Applications (MTAP) Journal**](https://link.springer.com/journal/11042)! 🗣️

- **September 2026**: I started a six-month research internship abroad at the [**MIS Laboratory at UPJV**](https://www.mis.u-picardie.fr/) (Amiens, France 🇫🇷), under the supervision of [**Prof. Florence Levé**](https://scholar.google.com/citations?user=0wuLEUwAAAAJ&hl=fr)!

- **February 2026**: The preprint of our work [**Art2Mus: Artwork-to-Music Generation via Visual Conditioning and Large-Scale Cross-Modal Alignment**](https://arxiv.org/abs/2602.17599) is now available on arXiv! 🎨🎹

- **February 2026**: Our work, [**Handscribe: A Gloss-Free Framework for Sign Language Translation and Gloss Sequence Generation**](https://doi.org/10.1016/j.cviu.2026.104674), was accepted for publication in the [**Computer Vision and Image Understanding (CVIU) Journal**](https://www.sciencedirect.com/journal/computer-vision-and-image-understanding)! 🖐🏻🤌🏻

- **July 2025**: I had the opportunity to attend the [**International Computer Vision Summer School (ICVSS2025)**](https://icvss.dmi.unict.it/icvss2025/Home) in Scicli (Ragusa), where I also presented a poster on my work [**Art2Mus: Bridging Visual Arts and Music through Cross-Modal Generation**](https://link.springer.com/chapter/10.1007/978-3-031-92808-6_11)! ☀️

- **May 2025**: The proceedings of my work, [**Art2Mus: Bridging Visual Arts and Music through Cross-Modal Generation**](https://link.springer.com/chapter/10.1007/978-3-031-92808-6_11), have been published by Springer! Feel free to check it out! ✨

- **October 2024**: We released a preprint of our work [**Art2Mus: Bridging Visual Arts and Music through Cross-Modal Generation**](https://arxiv.org/abs/2410.04906), which was recently presented at the [**AI4VA Workshop**](https://sites.google.com/view/ai4vaeccv2024) during [**ECCV 2024**](https://eccv.ecva.net/) in Milan this September! 🇮🇹 😎

- **August 2024**: Our work **Art2Mus: Bridging Visual Arts and Music through Cross-Modal Generation** was accepted at the [**AI4VA Workshop**](https://sites.google.com/view/ai4vaeccv2024) at [**ECCV 2024**](https://eccv.ecva.net/) in Milan! 🇮🇹

- **July 2024**: Our work [**Instructing and Prompting Large Language Models for Explainable Cross-domain Recommendations**](https://dl.acm.org/doi/10.1145/3640457.3688137) was accepted at [**RecSys 2024**](https://recsys.acm.org/recsys24/) in Bari! 🇮🇹

- **July 2024**: I **successfully defended my Master’s thesis** in Deep Learning at the [**University of Bari Aldo Moro**](https://www.uniba.it/en)! 💻

- **June 2024**: I attended [**AILC**](https://www.ai-lc.it/en/lectures-2/lectures-2024/) in Bari, where I deepened my knowledge of computational linguistics, digital humanities, and large language models! 🇮🇹

</div>

<div style="text-align:center;">
  <button id="news-toggle" class="news-btn" type="button" aria-expanded="false"></button>
</div>

<script>
(function () {
  var K = 5; // number of news items always visible
  var items = document.querySelectorAll('#news li');
  var btn = document.getElementById('news-toggle');
  if (!btn || items.length <= K) return;
  var expanded = false;
  function render() {
    items.forEach(function (li, i) {
      li.style.display = (expanded || i < K) ? '' : 'none';
    });
    btn.textContent = expanded ? 'Show less ▲' : 'Show ' + (items.length - K) + ' more ▼';
    btn.setAttribute('aria-expanded', expanded);
  }
  btn.style.display = 'block';
  btn.addEventListener('click', function () {
    expanded = !expanded;
    render();
  });
  render();
})();
</script>

<div style="text-align:center;">

## 🐚 That's all from my side! 🪸

Take a breather, watch the koi swim by, and let your thoughts flow like the ripples in the pond. You’ve earned it!

</div>

![](img/koi.gif)
