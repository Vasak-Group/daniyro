<script lang="ts">
  import loveIcon from "../assets/icons/lovew.gif";

  const he = "Dani";
  const she = "Rocio";
</script>

<section class="w-full pb-20 bg-white relative">
  <h1
    class="text-primary text-[90px] leading-[110px] font-light mb-0 text-center font-heading"
  >
    {he}
    <span
      class="h-15 w-15 rounded-full bg-primary text-white inline-block text-[40px] font-light leading-[60px]"
      >&amp;</span
    >
    {she}
  </h1>
</section>
<footer class="bg-tertiary text-white text-center py-6">
  <p class="text-sm font-semibold mt-2">
    © {new Date().getFullYear()} {he} & {she}. Mucho amor para compartir.
  </p>
  <p class="text-sm font-normal my-2">
    Creado con <img src={loveIcon} alt="Love Icon" class="inline-block w-4 h-4" /> por <a href="https://vasak.net.ar/" class="text-white underline">Vasak Group</a>
  </p>
</footer>