<script lang="ts">
	const list = [1, 2, 3, 4, 5];
</script>

<h1>Markuplint Issues #1286</h1>

<section>
	<h2>Error with hyphen</h2>
	<ul>
		{#each list as item, i (`${i}-`)}
			<li>{item}</li>
		{/each}
	</ul>
	<ul>
		{#each list as item, i (`${item}-`)}
			<li>{item}</li>
		{/each}
	</ul>
	<ul>
		{#each list as item, i (`-${item}`)}
			<li>{item}</li>
		{/each}
	</ul>
	<ul>
		{#each list as item, i (`${item}-${i}`)}
			<li>{item}</li>
		{/each}
	</ul>
</section>
