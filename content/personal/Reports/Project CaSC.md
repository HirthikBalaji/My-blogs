<div class="title-page">
  <div class="title-page-header">
    <h1>YOUR TITLE</h1>
    <h2>YOUR SUBTITLE</h2>
  </div>
  <div class="title-page-meta">
    <p><strong>Prepared by:</strong> Hirthik Balaji C</p>
    <p><strong>Version:</strong> 0.0.1a</p>
    <p><strong>Date:</strong> 2026-06-05</p>
  </div>
</div>
# your Content goes here


<script>
(function() {
  function reorder() {
    const titlePage = document.querySelector(".title-page");
    const toc = document.querySelector("nav.toc");
    if (titlePage && toc) {
      document.body.insertBefore(titlePage, toc);
    } else if (titlePage) {
      document.body.insertBefore(titlePage, document.body.firstChild);
    }
  }
  reorder();
  document.addEventListener("DOMContentLoaded", reorder);
  window.addEventListener("load", reorder);
})();
</script>
 