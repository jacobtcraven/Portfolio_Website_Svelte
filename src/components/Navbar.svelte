<script>
    export let links = [];
    export let logoSrc = 'C:\Users\jacob\Mega\Personal\jacobCravenFirebase\my-svelte-app3\images\JacobCravenLogo.png'; // Add a prop for the image source
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
    nav {
        padding: 0.5rem 2rem;
        display: flex;
        justify-content: space-between; /* Space between logo and links */
        align-items: center; /* Vertically center items */
        position: absolute;
        top: 0;
        right: 0;
        width: auto;
        background-color: #3b3b3b; /* Background color of the navbar */
        margin-right: 20px; /* Space from the right edge */
    }

    .logo {
        height: 200px; /* Adjust height as needed */
        margin-right: 20px; /* Space between logo and links */
    }

    ul {
        list-style: none;
        display: flex;
        gap: 1rem;
    }

    a {
        color: white; /* Set link font color to white */
        text-decoration: none;
        padding: 0.25rem 0.5rem;
        background-color: transparent; /* Ensure background is transparent by default */
        transition: background-color 0.3s ease, color 0.3s ease; /* Smooth transition for background and color */
        font-family: 'Poppins', sans-serif; /* Use the Poppins font */
        font-weight: bold; /* Makes the text bold */
        border-radius: 5px; /* Apply border radius in the normal state */
        letter-spacing: 0.05em; /* Increase letter spacing */
    }

    a:hover {
        background-color: #555; /* Change to a darker shade on hover */
        color: white; /* Keep the text color white on hover */
    }
</style>
