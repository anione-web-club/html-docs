
<script>
    import { getTitleName } from '$lib/util';
    const title = getTitleName('태그')
</script>

<svelte:head>
    <title>{title}</title>
</svelte:head>

<slot></slot>