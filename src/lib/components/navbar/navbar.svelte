<script>
  import EttyLogo from '$lib/styles/pictures/Etty.jpeg';
  import LanguagesScrolling from '$lib/components/tools/languages.scrolling.svelte';
  import LoginButton from '$lib/components/buttons/button.login.svelte';
</script>

<nav style="display: flex; align-items: center; justify-content: space-between;">
    <div class="One">
      <img src={EttyLogo} alt="Etty" width="60" height="60">
      <h1>ETTY</h1>
    </div>
    
    <div class="Two">
      <LanguagesScrolling/>
      <LoginButton/>
    </div>
  </nav>
  
  <style>
    img {
      margin-right: 5px;
      border-radius: 50%;
    }
  
    h1 {
      font-family: "Inter";
      color: #AEAEAE;
    }
  
    nav {
      background: linear-gradient(70deg, #0B0B0B, #181818);
    }
  
    .One {
      display: flex;
      align-items: center;
    }
  
    .Two {
      display: flex;
      align-items: center;
    }
</style>
  