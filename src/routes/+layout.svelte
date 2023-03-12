<script>
    import { Styles } from 'sveltestrap';
    import { Header } from '$lib/ui';

    import { getTitleName } from '$lib/util';
    const title = getTitleName('HTML 문서')
</script>

<svelte:head>
    <title>{title}</title>
</svelte:head>

<Styles></Styles>

<Header></Header>

<slot></slot>