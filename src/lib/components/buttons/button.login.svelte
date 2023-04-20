<script>
    import DiscordIcons from '$lib/styles/icons/Discord.png';
    import { langStore } from '$lib/store.js';

  </script>

<ul style="display: flex; align-items: center;">
    <img src={DiscordIcons} alt="Discord" width="20" height="42" style="margin-right: 5px;">

    {#if $langStore === "fr"}
        <h1>Se connecter</h1>
    {:else if $langStore === "en"}
        <h1>Login</h1>
    {/if}

</ul>
  
<style>
  
    h1 {
        font-family: "Inter";
        text-align: center;
        font-size: 16px;
        color: #ffffff;
    }
  
    ul {
        margin-left: 50px;
        background-color: #464AB4;
        border-radius: 42px;
        cursor: pointer;
        transition: background-color 0.3s ease-in-out;
    }

    ul:hover {
        background-color: #343786;
    }
  
</style>