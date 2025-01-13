<script>
  export let margin = '20mm'; // Default margin value
</script>

<div class="page" style="padding: {margin};">
  <slot></slot>
</div>

<style>
  .page {
    width: 210mm;
    height: 297mm;
    background: white;
    margin: 10mm auto;
    box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
    box-sizing: border-box;
  }

  @media print {
    .page {
      width: auto;
      height: auto;
      padding: 0;
      margin: 0;
      box-shadow: none;
    }
  }
</style>
