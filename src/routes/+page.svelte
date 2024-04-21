<script>
import NavHost from '../components/molecules/NavHost.svelte';
import Hero from '../components/organisms/Hero.svelte';
import About from '../components/organisms/About.svelte';
import Art from '../components/organisms/Art.svelte';
import Repos from '../components/organisms/Repos.svelte';
import Supporters from '../components/organisms/Supporters.svelte';
import Companies from '../components/organisms/Companies.svelte';
import Videos from '../components/organisms/Videos.svelte';
import Threed from '../components/organisms/Threed.svelte';
import Footer from '../components/molecules/Footer.svelte';
</script>

<NavHost />
<main>
    <Hero />
    <About />
    <Companies />
    <Art />
    <Videos />
    <Threed />
    <!-- <Repos />
    <Supporters /> -->
    <Footer />
</main>
