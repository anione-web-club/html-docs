<script>
    import { Styles } from 'sveltestrap/src';
    import { Header } from '$lib/ui';

    import { getTitleName } from '$lib/util';
    import { page } from '$app/stores'
    const title = getTitleName($page.data.title)
</script>

<svelte:head>
    <title>{title}</title>
</svelte:head>

<Styles></Styles>

<Header></Header>

<main>
    <slot></slot>
</main>