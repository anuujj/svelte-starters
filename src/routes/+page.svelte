<script>
  import Para from "./Para.svelte";
  let name = "Anuj";
  let htmlString = "this is a <em>emphasis</em> text";
  let src = "/favicon.png";
  let description = "this is description from main page";
  let groceryList = ["tomato", "onion", "potato", "eggs", "milk", "oil"];
</script>

<h1>Welcome {name}</h1>
<img {src} alt="svelte fav-icon" />
<p>
  {@html htmlString}
</p>
<ul>
  {#each groceryList as item (item)}
    <li>{item}</li>
  {/each}
</ul>
<Para {description} />

<style>
  p {
    background-color: antiquewhite;
    border: 1px solid rgb(48, 47, 47);
    padding: 1em;
  }
  ul{
    list-style: none;
    padding: 1em;
  }
</style>
