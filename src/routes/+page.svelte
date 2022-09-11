<script lang="ts">
	const pi = Math.PI;
    const animals_i_love = [ "aardvarks", "dogs", "cats", "geckos", "snakes", "rabbits" ];
</script>

<h1>Hello, this is the first header</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<p>The value of pi is {pi}</p>

<p>Here's a list of animals I love:</p>
<ul>
{#each animals_i_love.sort((a, b) => a.length - b.length) as animal}
<li>{animal}</li>
{/each}
</ul>
