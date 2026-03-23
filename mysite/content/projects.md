---
Title: Projects
---

<br>

<h1 style="font-size:3.5rem; margin:0 0 -0.2em;">Projects</h1>

This is a summary / intro paragraph about the projects I have made. I really enjoy doing personal projects in my spare time. I always have so many ideas and I find it so fun to be able to implement them into real life. I'm always thinking about new ideas or ways to improve my projects / solving problems.

<br>

<!-- <hr style="border:none; border-top:1px solid #e0e0e0; margin:0 0 3.5rem;"> -->

<!-- ─── PROJECT 01 ─────────────────────────────────────────── -->

## 3DS MPO Wobble Tool

### <a href="https://github.com/chriskersov/3DS-wobble-gif" target="_blank" style="color:black; text-decoration:underline;">Link</a>&nbsp;-----&nbsp;<a href="https://github.com/chriskersov/3DS-wobble-gif" target="_blank" style="color:black; text-decoration:underline;">GitHub</a>

Streamlit, Pillow, NumPy, Streamlit Community Cloud

<div style="display:grid; grid-template-columns:1fr 1fr; gap:3rem; align-items:start; margin-bottom:1.75rem;">

<div>

A web tool for converting Nintendo 3DS MPO stereo images into animated wobble GIFs. Upload an MPO file, adjust the wobble speed and frame count, and download the result — all in the browser with no installation required. Built and deployed on Streamlit Community Cloud.

</div>

<div>

<div id="carousel" style="position:relative; width:100%;">
  <img id="carousel-img" src="/projects/screenshot1.png" alt="Project screenshot" style="width:100%; display:block; border:1px solid #e8e8e8;">
  <div style="display:flex; justify-content:center; align-items:center; gap:1rem; margin-top:0.5rem;">
    <button onclick="prevSlide()" style="background:none; border:none; cursor:pointer; font-size:1rem; color:#999;">&#8592;</button>
    <span id="carousel-counter" style="font-size:0.75rem; color:#999;">1 / 3</span>
    <button onclick="nextSlide()" style="background:none; border:none; cursor:pointer; font-size:1rem; color:#999;">&#8594;</button>
  </div>
</div>

</div>

</div>

<div id="readme-container" style="max-height:500px; overflow-y:auto; border:1px solid #e8e8e8; background:#f9f9f9; padding:1rem 1.25rem; margin-top:0.5rem;">
  <div id="readme-content" style="font-family:monospace; font-size:0.72rem; line-height:1.7; color:#666; margin:0; white-space:pre-wrap; word-break:break-word;">Loading README...</div>
</div>

<hr style="border:none; border-top:1px solid #e0e0e0; margin:3.5rem 0;">

<style>
  details[open] summary .arrow { display: none; }
  details:not([open]) summary .open-arrow { display: none; }
  details[open] #readme-container { max-height:none; }
</style>

<script src="https://cdn.jsdelivr.net/npm/marked/marked.min.js"></script>

<script>
const slides = [
  "/projects/screenshot1.png",
  "/projects/screenshot2.png",
  "/projects/wobble.gif"
];
let current = 0;

function updateCarousel() {
  document.getElementById("carousel-img").src = slides[current];
  document.getElementById("carousel-counter").textContent = (current + 1) + " / " + slides.length;
}
function nextSlide() { current = (current + 1) % slides.length; updateCarousel(); }
function prevSlide() { current = (current - 1 + slides.length) % slides.length; updateCarousel(); }

fetch("https://raw.githubusercontent.com/chriskersov/3DS-wobble-gif/main/README.md")
  .then(r => r.text())
  .then(text => { document.getElementById("readme-content").innerHTML = marked.parse(text); })
  .catch(() => { document.getElementById("readme-content").textContent = "Could not load README."; });
</script>

<!-- ─── PROJECT 02 ─────────────────────────────────────────── -->

<p style="font-size:0.75rem; letter-spacing:0.12em; text-transform:uppercase; color:#999; margin:0 0 0.4em;">Project 02</p>

## Project Name &nbsp;—&nbsp; [GitHub ↗](https://github.com)

<p style="font-family:monospace; font-size:0.8rem; color:#999; margin:-1rem 0 1.75rem;">TypeScript &nbsp;·&nbsp; React &nbsp;·&nbsp; Vite</p>

<div style="display:grid; grid-template-columns:1fr 1fr; gap:3rem; align-items:start; margin-bottom:1.75rem;">

<div>

Description of the project goes here. A lightweight component library with zero runtime dependencies. Built out of frustration with over-engineered alternatives — the entire thing is tree-shakeable and fully typed from end to end.

<p style="margin-top:1rem;">
<a href="https://github.com" style="font-size:0.8rem; letter-spacing:0.06em; text-transform:uppercase;">GitHub ↗</a>
</p>

</div>

<div>

<img src="/images/screenshot4.png" alt="Project screenshot" style="width:100%; display:block; border:1px solid #e8e8e8;">

</div>

</div>

<div style="margin-top:0.25rem;">
<p style="font-size:0.7rem; letter-spacing:0.12em; text-transform:uppercase; color:#bbb; margin:0 0 0.5em; display:flex; align-items:center; gap:0.75rem;">readme <span style="flex:1; height:1px; background:#e8e8e8; display:inline-block;"></span></p>
<pre style="font-family:monospace; font-size:0.72rem; line-height:1.7; color:#666; background:#f9f9f9; border:1px solid #e8e8e8; padding:1rem 1.25rem; margin:0; overflow-x:auto; white-space:pre;"># Project Name

Zero-dependency component library for React.

## Quick start

    npm install project-name

All components are fully typed and 100% accessible.
No runtime CSS-in-JS. Ships as plain ESM.</pre>

</div>

<hr style="border:none; border-top:1px solid #e0e0e0; margin:3.5rem 0;">

<!-- ─── PROJECT 03 ─────────────────────────────────────────── -->

<p style="font-size:0.75rem; letter-spacing:0.12em; text-transform:uppercase; color:#999; margin:0 0 0.4em;">Project 03</p>

## Project Name &nbsp;—&nbsp; [GitHub ↗](https://github.com)

<p style="font-family:monospace; font-size:0.8rem; color:#999; margin:-1rem 0 1.75rem;">Rust &nbsp;·&nbsp; WASM</p>

<div style="display:grid; grid-template-columns:1fr 1fr; gap:3rem; align-items:start; margin-bottom:1.75rem;">

<div>

Description of the project goes here. Compiled to WebAssembly for near-native performance in the browser. An experiment in pushing what's possible on the client side without any JavaScript runtime overhead.

<p style="margin-top:1rem;">
<a href="https://github.com" style="font-size:0.8rem; letter-spacing:0.06em; text-transform:uppercase;">GitHub ↗</a>
</p>

</div>

<div>

<img src="/images/screenshot5.png" alt="Project screenshot" style="width:100%; display:block; border:1px solid #e8e8e8;">

</div>

</div>

<div style="margin-top:0.25rem;">
<p style="font-size:0.7rem; letter-spacing:0.12em; text-transform:uppercase; color:#bbb; margin:0 0 0.5em; display:flex; align-items:center; gap:0.75rem;">readme <span style="flex:1; height:1px; background:#e8e8e8; display:inline-block;"></span></p>
<pre style="font-family:monospace; font-size:0.72rem; line-height:1.7; color:#666; background:#f9f9f9; border:1px solid #e8e8e8; padding:1rem 1.25rem; margin:0; overflow-x:auto; white-space:pre;"># Project Name

Browser-native performance via WebAssembly.

## Build

    wasm-pack build --target web

Zero JS runtime overhead.
Integrates with any frontend framework.</pre>

</div>

<br>
