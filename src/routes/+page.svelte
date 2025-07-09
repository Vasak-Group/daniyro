<script lang="ts">
  import Contdown from '../components/sections/contdown.svelte';
  import Fontpage from '../components/sections/fontpage.svelte';
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

