<script>
  import Navbar from './components/Navbar.svelte';
  import './styles/global.css'
  import './styles/fonts.css'
  import { Router } from 'svelte-routing';

  const links = [
          { name: 'Home', href: '/' },
          { name: 'About', href: '/about' },
          { name: 'Contact', href: '/contact' }
  ];

</script>

<Navbar {links} />

<!--<Router>-->
<!--  <Home path="/" />-->
<!--  <About path="/about" />-->
<!--  <Projects path="/projects" />-->
<!--  <Contact path="/contact" />-->
<!--</Router>-->

<main>
  <h1>Welcome to my Svelte app!</h1>
  <p>This is a simple Svelte app with routing.</p>
</main>
