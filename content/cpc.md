---
date: 2016-10-12
title: Copy-pastable characters
type: page
aliases: emoji
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
    <dt>Text</dt>
      <dd title="LEFT-POINTING DOUBLE ANGLE QUOTATION MARK (U+00AB)" data-clipboard-text="«">«</dd>
      <dd title="MIDDLE DOT (U+00B7)" data-clipboard-text="·">·</dd><!-- General use—NOT U+22C5 -->
      <dd title="RIGHT-POINTING DOUBLE ANGLE QUOTATION MARK (U+00BB)" data-clipboard-text="»">»</dd>
      <dd title="RIGHT SINGLE QUOTATION MARK (U+2019)" data-clipboard-text="’">’</dd>
      <dd title="LEFT DOUBLE QUOTATION MARK (U+201C)" data-clipboard-text="“">“</dd>
      <dd title="RIGHT DOUBLE QUOTATION MARK (U+201D)" data-clipboard-text="”">”</dd>
      <dd title="EN DASH (U+2013)" data-clipboard-text="–">–</dd>
      <dd title="EM DASH (U+2014)" data-clipboard-text="—">—</dd>
      <dd title="HORIZONTAL ELLIPSIS (U+2026)" data-clipboard-text="…">…</dd>
      <dd title="DOT OPERATOR (U+22C5)" data-clipboard-text="⋅">⋅</dd><!-- Math use—NOT U+00B7 -->
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