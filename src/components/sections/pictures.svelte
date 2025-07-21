<script lang="ts">
  import emblaCarouselSvelte from "embla-carousel-svelte";
  import Autoplay from "embla-carousel-autoplay";

  import curvasIMG from "../../assets/img/curvas02.svg";
  import cameraIcon from "../../assets/icons/camera.gif";
  import carousel01 from "../../assets/img/carousel/1.png";
  import carousel02 from "../../assets/img/carousel/2.jpg";
  import carousel03 from "../../assets/img/carousel/3.jpg";

  const options = {
    loop: true,
    speed: 10,
    draggable: true,
    dragFree: false,
  };
  const plugins = [Autoplay()];

  const slides = [
    { src: carousel01, alt: "Imagen 1" },
    { src: carousel02, alt: "Imagen 2" },
    { src: carousel03, alt: "Imagen 3" },
  ];
</script>

<section
  class="relative h-[80%] mt-10 bg-white flex justify-center align-items-center"
>
  <img
    class="absolute bg-center -top-[85px] md:-top-[135px] lg:-top-[180px] xl:-top-[220px] z-0 w-full"
    src={curvasIMG}
    alt="Curvas decorativas"
  />

  <div class="flex justify-center align-items-center text-center z-10 pt-20">
    <div class="">
      <h2
        class="font-heading inline-block text-[60px] leading-16 mb-0 text-primary"
      >
        Retratos de Nuestro Amor
      </h2>
      <p class="w-full text-primary inline-block text-xl font-normal">
        Un minuto, un segundo, un instante que queda en la eternidad
      </p>

      <div class="w-20 mx-auto">
        <img
          class="w-full h-auto mt-10"
          src={cameraIcon}
          alt="Cámara"
          loading="lazy"
        />
      </div>

      <div class="pt-10 inline-block w-full">
        <div class="embla" use:emblaCarouselSvelte={{ options, plugins }}>
          <div class="flex">
            {#each slides as slide}
              <div class="embla__slide p-10">
                <div class="p-4 bg-[#f5f5f5] pb-24 shadow-lg rounded">
                  <img class="w-full h-auto" src={slide.src} alt={slide.alt} />
                </div>
              </div>
            {/each}
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
  .embla {
    overflow: hidden;
  }
  .embla__slide {
    flex: 0 0 33%;
    min-width: 0;
  }

  @media (max-width: 768px) {
    .embla__slide {
      flex: 0 0 100%;
    }
  }
</style>
