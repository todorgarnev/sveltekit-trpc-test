<script lang="ts">
	import type { PageData } from "./$types";

	export let data: PageData;
</script>

<h4>Data loaded in<br /><code>+page.ts</code></h4>
<p>{data.greeting}</p>

{#each data.posts as post}
	<div>{post.name}: {post.age}</div>
{/each}
