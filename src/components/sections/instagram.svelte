<script>
  import instagramIcon from "../../assets/icons/instagram.gif";
  import lineasTIMG from "../../assets/img/lineas03.svg";
  import lineasBIMG from "../../assets/img/lineas04.svg";

  const hashtag = "#daniyro";
</script>

<section class="relative flex flex-col justify-center items-center">
  <img class=" z-0 w-full" src={lineasTIMG} alt="Curvas decorativas" />
  <div class="row text-center d-flex justify-content-center align-items-center">
    <h2
      class="font-heading inline-block text-[60px] leading-16 mb-0 text-primary"
    >
      Compartimos este día junto a vos
    </h2>
    <p class="w-full text-primary inline-block text-xl font-normal">
      Compartí tus fotos y videos de ese hermoso día
    </p>

    <div class="w-full flex justify-center align-items-center">
      <img src={instagramIcon} alt="Instagram icon" class="w-[80px] h-auto my-6 " />
    </div>

    <div class="w-full text-center">
      <a target="_blank" href="https://www.instagram.com/" class="mb-10 font-bold text-secondary lowercase text-6xl inline-block"
        >{hashtag}</a
      >
    </div>

    <a target="_blank" href="https://www.instagram.com/" class="bg-tertiary w-auto text-white uppercase rounded-full font-bold px-6 py-4 text-[15px] mt-8 inline-block mb-16"
      >Ver en Instagram</a
    >
  </div>
  <img class="z-0 w-full" src={lineasBIMG} alt="Curvas decorativas" />
</section>
