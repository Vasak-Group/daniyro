<script lang="ts">
  import comillasInicio from "../../assets/img/comilla-apertura.svg";
  import comillasFin from "../../assets/img/comilla-cierre.svg";
  import grupo01a from "../../assets/img/Grupo01_a.png";
  import grupo01b from "../../assets/img/Grupo01_b.png";
  import grupo01c from "../../assets/img/Grupo01_c.png";

  const { he, she, date } = $props();
</script>

<!-- Portada -->
<section class="w-full pb-50 bg-cover relative">
  <img
    class="absolute w-90 h-auto -top-22 left-0 right-0 mx-auto z-[1]"
    src={grupo01a}
    alt=""
    loading="lazy"
  />

  <img
    class="absolute w-90 h-auto -top-22 left-0 right-0 mx-auto z-[2]"
    src={grupo01b}
    alt=""
    loading="lazy"
  />

  <img
    class="absolute w-90 h-auto -top-22 left-0 right-0 mx-auto"
    src={grupo01c}
    alt=""
    loading="lazy"
  />

  <div class="flex justify-center align-items-center">
    <div class="relative z-40 w-[75%] text-center">
      <div class="pt-44">
        <span class="text-primary table no-wrap w-full font-light text-2xl">
          {date.getDate()}.{date.getMonth() + 1}.{date.getFullYear()}
        </span>
        <h1
          class="text-primary text-[130px] leading-[110px] font-light mb-0 text-center font-heading flex flex-col justify-center items-center lg:flex-row"
        >
          {he}
          <span
            class="h-15 w-15 rounded-full bg-primary text-white text-[40px] font-light leading-[60px] lg:mx-4"
            >&amp;</span
          >
          {she}
        </h1>
        <div class="w-[50%] mx-auto mt-6 h-[1px] bg-primary"></div>
      </div>

      <div class="pt-9">
        <p>
          <img
            class="inline-block w-8 h-8 my-2.5"
            src={comillasInicio}
            alt=""
          /> <br />

          El amor es la razón de este día <br />

          <img class="inline-block w-8 h-8 my-2.5" src={comillasFin} alt="" />
        </p>
      </div>
    </div>
  </div>
</section>
