<script>
  export let name;
  import Buttons from "./Buttons.svelte";
</script>

<style>
  h1 {
    color: purple;
  }
</style>

<h1>Hello {name}!</h1>
<hr />
<Buttons />
