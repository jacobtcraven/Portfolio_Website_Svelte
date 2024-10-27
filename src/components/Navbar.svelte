<script>
    export let links = [];
    export let logoSrc = '../images/JacobCravenLogoCropped.png'; // Add a prop for the image source
</script>

<nav>
    <img src={logoSrc} alt="Logo" class="logo" />
    <ul>
        {#each links as link}
            <li><a href={link.href} rel="prefetch">{link.name}</a></li>
        {/each}
    </ul>
</nav>

<style>
    
</style>
