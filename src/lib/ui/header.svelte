<script>
    import { Navbar, NavbarBrand, Collapse, Nav, NavItem, NavLink, NavbarToggler } from 'sveltestrap';
    import { base } from '$app/paths';

    let isOpen = false
    function toggle() {
        isOpen = !isOpen
    }
</script>

<Navbar color='dark' dark class='me-auto'>
    <NavbarBrand href='{base}/'>HTML</NavbarBrand>
    <NavbarToggler on:click={toggle} />
    <Collapse {isOpen} navbar>
        <Nav navbar>
            <NavItem>
                <NavLink href='{base}/tag'>태그</NavLink>
            </NavItem>
        </Nav>
    </Collapse>
</Navbar>
