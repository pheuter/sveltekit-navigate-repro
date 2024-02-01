<script lang="ts">
	let { children, data } = $props();

	$inspect(data.membership);
</script>

<h1>{data.membership.workspaceName}'s Home</h1>

{#if data.membership.isAdmin}
	<p>You're an admin!</p>
{/if}

{@render children()}
