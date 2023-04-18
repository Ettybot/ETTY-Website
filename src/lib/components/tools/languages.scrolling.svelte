<script>
	let lang = "fr";
</script>

<select bind:value={lang}>
	<option value="fr">FR</option>
	<option value="en">EN</option>
</select>

{#if lang === "fr"}
    <p>Bonjour, comment ça va ?</p>
{:else if lang === "en"}
    <p>Hello, how are you?</p>
{/if}
