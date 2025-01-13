<div class="pages-container">
  <slot></slot>
</div>

<style>
  .pages-container {
    display: flex;
    flex-direction: column;
    gap: 20px;
    padding: 20px;
    background-color: #f0f0f0;
    min-height: 100vh;
  }

  @media print {
    .pages-container {
      padding: 0;
      gap: 0;
      background-color: transparent;
    }

    :global(.page) {
      break-inside: avoid;
      break-after: always;
    }

    :global(.page:last-child) {
      break-after: avoid;
    }

    @page {
      size: A4;
      margin: var(--page-margin, 20mm);
    }
  }
</style>
