---
date: 2016-10-12
title: Unicode copy-pastable characters
type: page
aliases:
  - cpc
  - ucpc
---

<div id="emoji">

<style scoped>
  dl, dt, dd { margin: 0; }
  dd {
    display: inline-block;
    min-width: 2rem;
    text-align: center;
    border: 1px solid #eee;
    font-size: xx-large;
  }
  dd:active {
    background: #fe9;
  }

</style>

<section id="textual">
<h1>Textual</h1>

<dl>
  <dt data-range="U+0080–U+00FF">Latin-1 Supplement</dt>
    <dd title="U+00AB « left-pointing double angle quotation mark" data-clipboard-text="«">«</dd>
    <dd title="U+00B7 · middle dot" data-clipboard-text="·">·</dd><!-- ≠ U+22C5 -->
    <dd title="U+00BB » right-pointing double angle quotation mark" data-clipboard-text="»">»</dd>
  <dt data-range="U+2000–U+206F">General Punctuation</dt>
    <dd title="U+2019 ’ right single quotation mark" data-clipboard-text="’">’</dd>
    <dd title="U+201C “ left double quotation mark" data-clipboard-text="“">“</dd>
    <dd title="U+201D ” right double quotation mark" data-clipboard-text="”">”</dd>
    <dd title="U+2013 – en dash" data-clipboard-text="–">–</dd>
    <dd title="U+2014 — em dash" data-clipboard-text="—">—</dd>
    <dd title="U+2026 … horizontal ellipsis" data-clipboard-text="…">…</dd>
  <dt data-range="U+2200–U+22FF">Mathematical Operators</dt>
    <dd title="U+2248 ≈ almost equal to" data-clipboard-text="≈">≈</dd>
    <dd title="U+2260 ≠ not equal to" data-clipboard-text="≠">≠</dd>
    <dd title="U+22C5 ⋅ dot operator" data-clipboard-text="⋅">⋅</dd><!-- ≠ U+00B7 -->
  </dl>
</section>

<section id="emoji">
<h1>Emoji</h1>

  <dt>Smileys & People</dt>
    <!-- face-positive -->
    <dd title="U+1F600 😀 grinning face" data-clipboard-text="😀">😀</dd>
    <dd title="U+1F601 😁 grinning face with smiling eyes" data-clipboard-text="😁">😁</dd>
    <dd title="U+1F602 😂 face with tears of joy" data-clipboard-text="😂">😂</dd>
    <dd title="U+1F923 🤣 rolling on the floor laughing" data-clipboard-text="🤣">🤣</dd>
    <dd title="U+1F603 😃 smiling face with open mouth" data-clipboard-text="😃">😃</dd>
    <dd title="U+1F604 😄 smiling face with open mouth &amp; smiling eyes" data-clipboard-text="😄">😄</dd>
    <dd title="U+1F605 😅 smiling face with open mouth &amp; cold sweat" data-clipboard-text="😅">😅</dd>
    <dd title="U+1F606 😆 smiling face with open mouth &amp; closed eyes" data-clipboard-text="😆">😆</dd>
    <dd title="U+1F609 😉 winking face" data-clipboard-text="😉">😉</dd>
  
  <dt>Animals & Nature</dt>
    <!-- animal-mammal -->
    <dd title="U+1F987 🦇 bat" data-clipboard-text="🦇">🦇</dd>
    <!-- animal-bird -->
    <dd title="U+1F427 🐧 penguin" data-clipboard-text="🐧">🐧</dd>
    <dd title="U+1F989 🦉 owl" data-clipboard-text="🦉">🦉</dd>

  <dt>Travel & Places</dt>
    <!-- transport-ground -->
    <dd title="U+1F6F4 🛴 kick scooter" data-clipboard-text="🛴">🛴</dd>
    <dd title="U+1F6D1 🛑 stop sign" data-clipboard-text="🛑">🛑</dd>
</section>

</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/clipboard.js/1.5.12/clipboard.min.js"></script>

<script>
var elems = document.querySelectorAll('#emoji > dl > dd');
var clipboard = new Clipboard(elems);
clipboard.on('success', function(e) {
  console.log(e);
});
clipboard.on('error', function(e) {
  console.log(e);
});
</script>