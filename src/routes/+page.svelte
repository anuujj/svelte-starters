<script>
  import Para from './Para.svelte';
  let name = "Anuj";
  let htmlString = "this is a <em>emphasis</em> text";
  let src = "/favicon.png";
  let description = "this is description from main page";
</script>

<h1>Welcome {name}</h1>
<img {src} alt="svelte fav-icon" />
<p>
  Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation
  {@html htmlString}
</p>
<Para {description}/>

<style>
  p {
    background-color: antiquewhite;
    border: 1px solid rgb(48, 47, 47);
    padding: 1em;
  }
</style>
