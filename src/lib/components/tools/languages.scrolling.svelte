<script>
  import EnFlag from '$lib/styles/pictures/En_flag.jpeg';
  import FrFlag from '$lib/styles/pictures/Fr_flag.jpeg';
  import { langStore } from '$lib/store.js';

  let lang = "en";
  $: langStore.set(lang);
</script>

<select bind:value={lang} on:change={() => langStore.set(lang)}>

  <option value="fr">FR</option>
  <option value="en">EN</option>

</select>

{#if lang === "fr"}
  <img src={FrFlag} alt="Flag" width="25" height="25">
{:else if lang === "en"}
  <img src={EnFlag} alt="Flag" width="25" height="25">
{/if}

<style>

  img {
    border-radius: 50%;
  }

  select {
    background: none;
    border: none;

    color: #AEAEAE;
  }

  option {
    font-family: "Inter ExtraBold";
    color: #AEAEAE;
  }

</style>