<script>
    import { 
        Navbar, 
        NavbarBrand, 
        Collapse, 
        Nav, 
        NavbarToggler, 
        DropdownToggle, 
        Dropdown, 
        DropdownMenu, 
        DropdownItem 
    } from 'sveltestrap/src';
    import { base } from '$app/paths';

    /** @type {{
     * title: string,
     * route:string,
     * child: {
     * route: string
     * name: string
     * }[]
     * }[]} */
    export let contents = []

    let isOpen = false
    function toggle() {
        isOpen = !isOpen
    }
</script>

<Navbar color='dark' dark class='me-auto'>
    <NavbarBrand href='{base}/'>웹 프로그래밍 동아리</NavbarBrand>
    <NavbarToggler on:click={toggle} />
    <Collapse {isOpen} navbar>
        <Nav navbar>
            {#each contents as content}
            <Dropdown nav inNavbar>
                <DropdownToggle nav caret>
                    {content.title}
                </DropdownToggle>
                <DropdownMenu end>
                    <DropdownItem href='{base}/{content.route}'>{content.title}</DropdownItem>
                    <DropdownItem divider />
                    {#each content.child as element}
                        <DropdownItem href='{base}/{content.route}/{element.route}'>{element.name}</DropdownItem>
                    {/each}
                </DropdownMenu>
            </Dropdown>
            {/each}
        </Nav>
    </Collapse>
</Navbar>
