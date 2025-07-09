<script lang="ts">
  import curvasIMG from "../../assets/img/curvas01.svg";
  import giftIcon from "../../assets/icons/gift.gif"
</script>

<section class="relative flex flex-col justify-center items-center mt-10 bg-white">
  <img
    class="absolute bg-center -top-[85px] md:-top-[135px] lg:-top-[180px] xl:-top-[220px] z-0 w-full"
    src={curvasIMG}
    alt="Curvas decorativas"
  />

  <picture>
    <img
      class="absolute w-[200px] h-auto top-[280px] -left-[30px]"
      src="https://fixdate.io/modelo-invitacion/65/img/Grupo02_a.png"
      alt=""
      loading="lazy"
    />
  </picture>

  <picture>
    <img
      class="absolute w-[200px] h-auto top-[280px] -left-[30px]"
      src="https://fixdate.io/modelo-invitacion/65/img/Grupo02_b.png"
      alt=""
      loading="lazy"
    />
  </picture>

  <picture>
    <img
      class="absolute w-[200px] h-auto top-[280px] -left-[30px]"
      src="https://fixdate.io/modelo-invitacion/65/img/Grupo02_c.png"
      alt=""
      loading="lazy"
    />
  </picture>

  <div class="flex flex-col justify-center align-items-center z-10 text-center mt-20 mb-20">
    <h2 class="font-heading text-primary w-full inline-block text-center mb-0 text-[60px]">Regalos</h2>
    <p class="w-full text-primary inline-block text-xl font-normal">
      Si deseas regalarnos algo más que tu hermosa presencia...
    </p>

    <div class="w-full">
      <img
        class="w-[100px] h-auto mx-auto mt-10"
        src={giftIcon}
        alt="Regalos"
        loading="lazy"
      />
    </div>

    <a href="#" class="bg-tertiary w-auto text-white uppercase rounded-full font-bold px-6 py-4 text-[15px] mt-8">Ver más</a>
  </div>
</section>
