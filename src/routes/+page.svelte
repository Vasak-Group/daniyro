<script lang="ts">
  import Contdown from '../components/sections/contdown.svelte';
  import Date from '../components/sections/date.svelte';
  import Fest from '../components/sections/fest.svelte';
  import Fontpage from '../components/sections/fontpage.svelte';
  import Gift from '../components/sections/gift.svelte';
  import Instagram from '../components/sections/instagram.svelte';
  import Pictures from '../components/sections/pictures.svelte';
</script>

<!-- Background -->
<div class="h-screen w-screen fixed top-0 left-0 z-[-100] overflow-hidden">
  <img
    class="h-screen w-screen object-cover absolute top-0 left-0 z-[-100]"
    src="https://fixdate.io/modelo-invitacion/65/img/fondo.webp"
  />
</div>

<Fontpage />
<Contdown />
<Date />
<Pictures />
<Fest />
<Gift />
<Instagram />