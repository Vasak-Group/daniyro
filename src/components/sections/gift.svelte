<script lang="ts">
  import curvasIMG from "../../assets/img/curvas01.svg";
  import giftIcon from "../../assets/icons/gift.gif";
  import GiftModal from "../modals/giftModal.svelte";
  import grupo02aIMG from "../../assets/img/Grupo02_a.png";
  import grupo02bIMG from "../../assets/img/Grupo02_b.png";
  import grupo02cIMG from "../../assets/img/Grupo02_c.png";

  let isOpenGiftModal = false;
</script>

<section
  class="relative flex flex-col justify-center items-center mt-10 bg-white"
>
  <img
    class="absolute bg-center -top-[85px] md:-top-[135px] lg:-top-[180px] xl:-top-[220px] z-0 w-full"
    src={curvasIMG}
    alt="Curvas decorativas"
  />

  <img
    class="absolute w-[200px] h-auto top-[120px] -left-[30px] hidden lg:block"
    src={grupo02aIMG}
    alt=""
    loading="lazy"
  />

  <img
    class="absolute w-[200px] h-auto top-[120px] -left-[30px] hidden lg:block"
    src={grupo02bIMG}
    alt=""
    loading="lazy"
  />

  <img
    class="absolute w-[200px] h-auto top-[120px] -left-[30px] hidden lg:block"
    src={grupo02cIMG}
    alt=""
    loading="lazy"
  />

  <div
    class="flex flex-col justify-center align-items-center z-10 text-center mt-20 mb-20"
  >
    <h2
      class="font-heading text-primary w-full inline-block text-center mb-0 text-[60px]"
    >
      Regalos
    </h2>
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

    <button
      on:click={() => (isOpenGiftModal = true)}
      class="bg-tertiary w-auto text-white uppercase rounded-full font-bold px-6 py-4 text-[15px] mt-8 inline-block"
      >Ver más</button
    >
  </div>
</section>

{#if isOpenGiftModal}
  <GiftModal bind:isOpen={isOpenGiftModal} />
{/if}
