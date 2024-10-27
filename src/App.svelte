<script>
  import Navbar from './components/Navbar.svelte';
  import './styles/global.css';
  import './styles/fonts.css';
  import { Router } from 'svelte-routing';

  const links = [
      { name: 'Home', href: '/' },
      { name: 'About', href: '/about' },
      { name: 'Contact', href: '/contact' }
  ];
</script>

<Navbar {links} />

<main>
  <section class="hero">
    <img src="../images/HeadshotWebCircle2.png" alt="Jacob Craven" class="hero-image" />
    <h1>Jacob Craven</h1>
    <p>Student at Southern Illinois University Edwardsville</p>
  </section>
</main>

<style>
  /* Styles for the main section (cover photo area) */
  main {
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    color: black; /* Change text color to black */
    text-align: center;
  }

  .hero {
    width: 100%;
    padding: 2rem;
  }

  .hero-image {
    width: 100%; /* Adjust width as needed */
    max-width: 300px; /* Set a max width for the image */
    margin-bottom: 1rem; /* Space between image and text */
  }

  h1 {
    font-weight: bold; /* Make the font thicker */
    font-size: 3rem; /* Increase the font size for the header */
  }

  p {
    color: rgb(145, 0, 0); /* Ensure the paragraph text is also black */
    font-weight: bold;
    font-size: 1.5rem; /* Increase the font size for the paragraph */
  }
</style>
