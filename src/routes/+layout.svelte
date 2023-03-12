<script>
    import { getTitleName } from '$lib/util';
    const title = getTitleName('HTML 문서')
</script>

<svelte:head>
    <title>{title}</title>
</svelte:head>

<slot></slot>