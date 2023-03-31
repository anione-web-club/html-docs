<script>
    import { Styles } from 'sveltestrap/src';
    import { Header } from '$lib/ui';

    import { getTitleName } from '$lib/util';
    import { page } from '$app/stores'
    const title = getTitleName($page.data.title)
    const contents = [
        {
            title: '구조',
            route: 'structure',
            child: []
        },
        {
            title: '태그',
            route: 'tag',
            child: [
                { route: 'a', name: 'a'},
                { route: 'h1-h6', name: 'h1~h6'},
                { route: 'p', name: 'p'},
            ]
        },
    ]
</script>

<svelte:head>
    <title>{title}</title>
</svelte:head>

<Styles />

<Header 
    {contents}
/>

<main>
    <slot></slot>
</main>