<script>
  import PagesContainer from '$lib/base/PagesContainer.svelte';
  import Page from '$lib/base/Page.svelte';
</script>

<PagesContainer>
    
  <Page margin="15mm">
    <h1>Page 1</h1>
    <p>Content for Page 1</p>
  </Page>

  <Page margin="15mm">
    <h1>Page 2</h1>
    <p>Content for Page 2</p>
  </Page>
  <!-- Add more pages as needed -->
</PagesContainer>
