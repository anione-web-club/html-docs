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
    } from 'sveltestrap';
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
            <Dropdown nav inNavbar>
                <DropdownToggle nav caret>
                    태그
                </DropdownToggle>
                <DropdownMenu end>
                    <DropdownItem href='{base}/tag'>태그</DropdownItem>
                    <DropdownItem divider />
                    <DropdownItem href='{base}/tag/p'>p</DropdownItem>
                </DropdownMenu>
            </Dropdown>
        </Nav>
    </Collapse>
</Navbar>
