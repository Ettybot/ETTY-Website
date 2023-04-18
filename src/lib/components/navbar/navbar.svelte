<script>
  import EttyLogo from '/pictures/Etty.jpeg';
  import LanguagesScrolling from '$lib/components/tools/languages.scrolling.svelte';
  import LoginButton from '$lib/components/buttons/button.login.svelte';
</script>

<nav>
    <ul style="display: flex; align-items: center;">
        <img src={EttyLogo} alt="Etty" width="60" height="60">
        <h1>ETTY</h1>

        <LoginButton/>
    </ul>
</nav>

<style>

img {
    margin-right: 5px;
    border-radius: 50%;
}

h1 {
    color: #AEAEAE;
}

ul {
    height: 100px;
    background: linear-gradient(70deg, #0B0B0B, #181818);
}

</style>