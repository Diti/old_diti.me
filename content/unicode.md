---
date: 2016-10-12
title: Unicode copy-pastable characters
type: page
aliases:
  - cpc
  - emoji
  - ucpc
---

<div id="unicode">

<style scoped>
  dl, dt, dd { margin: 0; }
  dd {
    display: inline-block;
    min-width: 2rem;
    font-size: xx-large;
    text-align: center;
    vertical-align: middle;
    border: 1px solid #eee;
  }
  dd:active { background: #fe9; }
  dd img {
    max-width: 36px;
    max-height: 36px;
  }
</style>

<section id="textual">
<h1>Textual</h1>

<dl>
  <dt data-range="U+0080–U+00FF">Latin-1 Supplement</dt>
    <dd title="U+00AB « left-pointing double angle quotation mark">«</dd>
    <dd title="U+00B7 · middle dot">·</dd><!-- ≠ U+22C5 -->
    <dd title="U+00BB » right-pointing double angle quotation mark">»</dd>
  <dt data-range="U+2000–U+206F">General Punctuation</dt>
    <dd title="U+2019 ’ right single quotation mark">’</dd>
    <dd title="U+201C “ left double quotation mark">“</dd>
    <dd title="U+201D ” right double quotation mark">”</dd>
    <dd title="U+2013 – en dash">–</dd>
    <dd title="U+2014 — em dash">—</dd>
    <dd title="U+2026 … horizontal ellipsis">…</dd>
  <dt data-range="U+2200–U+22FF">Mathematical Operators</dt>
    <dd title="U+2248 ≈ almost equal to">≈</dd>
    <dd title="U+2260 ≠ not equal to">≠</dd>
    <dd title="U+22C5 ⋅ dot operator">⋅</dd><!-- ≠ U+00B7 -->
</dl>
</section>

<section id="emoji">
<h1>Emoji</h1>
<!-- The images used in this section come from https://commons.wikimedia.org/wiki/Emoji -->

<dl>
  <dt>Smileys & People</dt>
    <!-- face-positive -->
    <dd title="U+1F600 😀 grinning face"><img alt="😀" src="https://upload.wikimedia.org/wikipedia/commons/3/31/Emoji_u1f600.svg"></dd>
    <dd title="U+1F601 😁 grinning face with smiling eyes"><img alt="😁" src="https://upload.wikimedia.org/wikipedia/commons/c/cb/Emoji_u1f601.svg"></dd>
    <dd title="U+1F602 😂 face with tears of joy"><img alt="😂" src="https://upload.wikimedia.org/wikipedia/commons/1/1b/Emoji_u1f602.svg"></dd>
    <dd title="U+1F923 🤣 rolling on the floor laughing">🤣</dd>
    <dd title="U+1F603 😃 smiling face with open mouth"><img alt="😃" src="https://upload.wikimedia.org/wikipedia/commons/f/f9/Emoji_u1f603.svg"></dd>
    <dd title="U+1F604 😄 smiling face with open mouth &amp; smiling eyes"><img alt="😄" src="https://upload.wikimedia.org/wikipedia/commons/9/9d/Emoji_u1f604.svg"></dd>
    <dd title="U+1F605 😅 smiling face with open mouth &amp; cold sweat"><img alt="😅" src="https://upload.wikimedia.org/wikipedia/commons/5/53/Emoji_u1f605.svg"></dd>
    <dd title="U+1F606 😆 smiling face with open mouth &amp; closed eyes"><img alt="😆" src="https://upload.wikimedia.org/wikipedia/commons/2/24/Emoji_u1f606.svg"></dd>
    <dd title="U+1F609 😉 winking face"><img alt="😉" src="https://upload.wikimedia.org/wikipedia/commons/3/36/Emoji_u1f609.svg"></dd>
  
  <dt>Animals & Nature</dt>
    <!-- animal-mammal -->
    <dd title="U+1F987 🦇 bat">🦇</dd>
    <!-- animal-bird -->
    <dd title="U+1F427 🐧 penguin"><img alt="🐧" src="https://upload.wikimedia.org/wikipedia/commons/3/39/Emoji_u1f427.svg"></dd>
    <dd title="U+1F989 🦉 owl">🦉</dd>

  <dt>Travel & Places</dt>
    <!-- transport-ground -->
    <dd title="U+1F6F4 🛴 kick scooter">🛴</dd>
    <dd title="U+1F6D1 🛑 stop sign">🛑</dd>
</dl>
</section>

</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/clipboard.js/1.5.12/clipboard.min.js"></script>
<script>
  var elems = document.querySelectorAll('#unicode dd');
  new Clipboard(elems, {
    text: function(trigger) {
      var imgElems = trigger.getElementsByTagName('img'); 
      if (imgElems.length > 0) {
        return imgElems[0].getAttribute('alt'); // Emoji is an image, return its `alt` element
      } else {
        return trigger.textContent; // Emoji is plaintext, return its content
      }
    }
  });
</script>