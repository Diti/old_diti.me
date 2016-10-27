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
      display: table-cell;
      width: auto;
      min-width: 2rem;
      text-align: center;
      border: 1px solid #eee;
      font-size: xx-large;
    }
    dd:active {
      background: #fe9;
    }
  </style>

  <dl>
    <dt data-range="U+0080–U+00FF">Latin-1 Supplement</dt>
      <dd title="LEFT-POINTING DOUBLE ANGLE QUOTATION MARK (U+00AB)" data-clipboard-text="«">«</dd>
      <dd title="MIDDLE DOT (U+00B7)" data-clipboard-text="·">·</dd><!-- ≠ U+22C5 -->
      <dd title="RIGHT-POINTING DOUBLE ANGLE QUOTATION MARK (U+00BB)" data-clipboard-text="»">»</dd>
    <dt data-range="U+2000–U+206F">General Punctuation</dt>
      <dd title="RIGHT SINGLE QUOTATION MARK (U+2019)" data-clipboard-text="’">’</dd>
      <dd title="LEFT DOUBLE QUOTATION MARK (U+201C)" data-clipboard-text="“">“</dd>
      <dd title="RIGHT DOUBLE QUOTATION MARK (U+201D)" data-clipboard-text="”">”</dd>
      <dd title="EN DASH (U+2013)" data-clipboard-text="–">–</dd>
      <dd title="EM DASH (U+2014)" data-clipboard-text="—">—</dd>
      <dd title="HORIZONTAL ELLIPSIS (U+2026)" data-clipboard-text="…">…</dd>
    <dt data-range="U+2200–U+22FF">Mathematical Operators</dt>
      <dd title="ALMOST EQUAL TO (U+2248)" data-clipboard-text="≈">≈</dd>
      <dd title="NOT EQUAL TO (U+2260)" data-clipboard-text="≠">≠</dd>
      <dd title="DOT OPERATOR (U+22C5)" data-clipboard-text="⋅">⋅</dd><!-- ≠ U+00B7 -->
    <dt data-range="U+1F300–U+1F5FF">Miscellaneous Symbols and Pictographs</dt>
      <dd title="PENGUIN (U+1F427)" data-clipboard-text="🐧">🐧</dd>
    <dt data-range="U+1F900–U+1F9FF">Supplemental Symbols and Pictographs</dt>  
      <dd title="KICK SCOOTER (U+1F6F4)" data-clipboard-text="�">�</dd>
      <dd title="BAT (U+1F987)" data-clipboard-text="�">�</dd>
      <dd title="OWL (U+1F989)" data-clipboard-text="�">�</dd>
  </dl>
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