<nav>
    <div class="nav-container">
        <a href="/" class="nav-logo" title="Back to Homepage">Alex Nau</a>
        <a href="/"><img src=".\img\logo.png" alt="logo" class="toto"></a>
        <div class="nav-links">
            {#each nav as link}
                {#if link.isShow}
                    <a href={link.href} class="link">{link.title}</a>
                {/if}
            {/each}
        </div>
    </div>
</nav>
<div class="container">
    <slot></slot>
</div>

<script>
    const nav = [
        {
            title: 'About me',
            href: '/about',
            isShow: true,
        },
        {
            title: 'Blog',
            href: '/blog',
            isShow: true,
        },
        {
            title: 'My projects',
            href: '/project',
            isShow: true,
        },
    ]
</script>

<style>
    .container {
    max-width: 1400px;
    margin: 50px auto;
    }
    .toto {
        height: 100%;
        width: 100%;
    }
</style>