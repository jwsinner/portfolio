<script lang="ts">
    import {page} from '$app/stores';
</script>

<header>

    <nav>
        <ul>
            <li class:active={$page.path === '/'}><a sveltekit:prefetch href="/">Home</a></li>
            <li class:active={$page.path === '/about'}><a sveltekit:prefetch href="/about">About</a></li>
            <li class:active={$page.path === '/todos'}><a sveltekit:prefetch href="/todos">Todos</a></li>
        </ul>
    </nav>

    <div class="corner">
        <!-- TODO put something else here? github link? -->
    </div>
</header>

<style>
    header {
        display: flex;
        justify-content: center;
        height: 60px;
    }

    nav {
        display: flex;
        justify-content: center;
        --background: rgba(255, 255, 255, 0.7);
    }

    ul {
        position: relative;
        padding: 0;
        margin: 0;
        height: 3em;
        display: flex;
        justify-content: center;
        align-items: center;
        list-style: none;
        background: var(--background);
        background-size: contain;
    }

    li {
        position: relative;
        height: 100%;
    }

    nav a {
        display: flex;
        height: 100%;
        align-items: center;
        padding: 0 1em;
        color: var(--heading-color);
        font-weight: 700;
        font-size: 0.8rem;
        text-transform: uppercase;
        letter-spacing: 0.1em;
        text-decoration: none;
        transition: color 0.2s linear;
    }

    a:hover {
        color: var(--accent-color);
    }
</style>
