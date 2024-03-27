<script>
    import { onMount } from 'svelte';

    let isNavOpen = false;

    const toggleNav = () => {
        isNavOpen = !isNavOpen;
        if (isNavOpen) {
            document.body.classList.add('no-scroll');
        } else {
            document.body.classList.remove('no-scroll');
        }
    }

    const closeNav = () => {
        isNavOpen = false;
        document.body.classList.remove('no-scroll');
    }
</script>

<header class="blur">
    <nav>
        <router-link to="/" class="logo__link d-flex" on:click={closeNav}>
            <div class="personal__logo">Amir Amerian</div>
        </router-link>

        <div class="nav__menu nav__list">
            <ul class="nav__link--list nav__item">
                <li>
                    <a href="#techstack" class="nav__link nav__link--anchor link__hover-effect link__hover-effect--black">Technologie</a>
                </li>
                <li>
                    <a href="#projects" class="nav__link nav__link--anchor link__hover-effect link__hover-effect--black">Projecten</a>
                </li>
                <li>
                    <a href="mailto:matthijs.blauw@gmail.com" class="nav__link nav__link--anchor nav__link--anchor-primary">Contact</a>
                </li>
            </ul>
        </div>

<!--        <HamburgerMenu on:click={toggleNav} {isNavOpen} class="menu__trigger"></HamburgerMenu>-->
    </nav>
</header>

<style>
    /* Your existing CSS styles */
</style>

