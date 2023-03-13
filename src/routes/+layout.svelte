<script>
    import { Styles } from 'sveltestrap/src';
    import { Header } from '$lib/ui';

    import { getTitleName } from '$lib/util';
    import { page } from '$app/stores'
    const title = getTitleName($page.data.title)
    const tagList = ['p', 'a', 'h1'].sort()
</script>

<svelte:head>
    <title>{title}</title>
</svelte:head>

<Styles />

<Header 
    {tagList}
/>

<main>
    <slot></slot>
</main>