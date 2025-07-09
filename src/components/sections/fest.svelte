<script lang="ts">
  import linesIMG from "../../assets/img/lineas02.svg";

  const items = [
    {
      title: "Música",
      description:
        "¿Cuál es la canción que no debe faltar en la PlayList de la fiesta?",
      buttonText: "Sugerir canción",
      iconSrc: "https://fixdate.io/modelo-invitacion/65/img/Grupo03.png",
    },
    {
      title: "Dress Code",
      description: "Una orientación para tu vestuario",
      buttonText: "Ver Más",
      iconSrc: "https://fixdate.io/modelo-invitacion/65/img/Grupo04.png",
    },
    {
      title: "Tips y Notas",
      description: "Información adicional para tener en cuenta",
      buttonText: "+ Info",
      iconSrc: "https://fixdate.io/modelo-invitacion/65/img/Grupo05.png",
    },
  ];
</script>

<section
  class="relative pt-[14%] pb-[17%] flex justify-center items-center bg-white"
>
  <img
    src={linesIMG}
    alt="Decorative lines"
    class="absolute top-0 left-0 w-full h-auto mt-30"
  />
  <div class="flex flex-col justify-center align-items-center text-center">
    <div class="w-full mt-12">
      <h2
        class="font-heading text-primary w-full inline-block text-center mb-0 text-[60px]"
      >
        Fiesta
      </h2>
      <p class="w-full text-primary inline-block text-xl font-normal">
        Hagamos juntos una fiesta épica. Aquí algunos detalles a tener en
        cuenta.
      </p>
    </div>

    <div class="flex flex-wrap content-center justify-center">
      {#each items as item}
        <div class="mt-14 px-8 w-[420px]">
          <div
            class="px-6 py-12 bg-[#f5f5f5] shadow-lg rounded-2xl min-h-[400px] flex flex-col justify-between items-center"
          >
            <h3 class="font-bold text-primary text-2xl mb-2">{item.title}</h3>
            <img
              class="w-auto h-[70px] mb-4"
              src={item.iconSrc}
              alt={item.title}
              loading="lazy"
            />
            <p class="text-secondary font-normal">{item.description}</p>
            <button class="w-[85%] bg-tertiary text-white uppercase rounded-full font-bold px-6 py-4 text-[15px]">{item.buttonText}</button>
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>
