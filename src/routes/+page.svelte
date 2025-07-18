<script lang="ts">
  import Footer from "../components/footer.svelte";
  import Contdown from "../components/sections/contdown.svelte";
  import DateSection from "../components/sections/date.svelte";
  import Fest from "../components/sections/fest.svelte";
  import Fontpage from "../components/sections/fontpage.svelte";
  import Gift from "../components/sections/gift.svelte";
  import Instagram from "../components/sections/instagram.svelte";
  import Pictures from "../components/sections/pictures.svelte";

  const he = "Daniel";
  const she = "Rocio";
  const date = new Date("29 Nov 2025 18:00:00 GMT-0300");
</script>

<!-- Background -->
<div class="h-screen w-screen fixed top-0 left-0 z-[-100] overflow-hidden">
  <img
    class="h-screen w-screen object-cover absolute top-0 left-0 z-[-100]"
    src="https://fixdate.io/modelo-invitacion/65/img/fondo.webp"
    alt="Background paper"
  />
</div>

<Fontpage {he} {she} {date} />
<Contdown {date} />
<DateSection />
<Pictures />
<Fest />
<Gift />
<Instagram />
<Footer {he} {she} />