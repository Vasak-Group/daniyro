<script lang="ts">
  import linesIMG from "../../assets/img/lineas02.svg";
  import musicIcon from "../../assets/icons/music.gif";
  import dressIcon from "../../assets/icons/kimono.gif";
  import infoIcon from "../../assets/icons/document.gif";

  import DressModal from "../modals/dressModal.svelte";

  let isOpenDressModal = false;
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
        Hagamos juntos una fiesta épica. Acá van algunos detalles a tener en
        cuenta
      </p>
    </div>

    <div class="flex flex-wrap content-center justify-center">
      <div class="mt-14 px-8 w-[420px]">
        <div
          class="px-6 py-12 bg-[#f5f5f5] shadow-lg rounded-2xl min-h-[400px] flex flex-col justify-between items-center"
        >
          <h3 class="font-bold text-primary text-2xl mb-2">Música</h3>
          <img
            class="w-auto h-[70px] mb-4"
            src={musicIcon}
            alt="Música"
            loading="lazy"
          />
          <p class="text-secondary font-normal">
            ¿Cuál es la canción que no debe faltar en la PlayList de la fiesta?
          </p>
          <a
            href="https://open.spotify.com/playlist/5YfUrhlal1kB4IBHLFpQDX?si=MDvPtqgTTtG8dOF_ae4uFg&utm_source=whatsapp"
            target="_blank"
            rel="noopener noreferrer"
            class="w-[85%] bg-tertiary text-white uppercase rounded-full font-bold px-6 py-4 text-[15px]"
            >Sugerir canción</a
          >
        </div>
      </div>

      <div class="mt-14 px-8 w-[420px]">
        <div
          class="px-6 py-12 bg-[#f5f5f5] shadow-lg rounded-2xl min-h-[400px] flex flex-col justify-between items-center"
        >
          <h3 class="font-bold text-primary text-2xl mb-2">Dress Code</h3>
          <img
            class="w-auto h-[70px] mb-4"
            src={dressIcon}
            alt="Dress Code"
            loading="lazy"
          />
          <p class="text-secondary font-normal">
            Una orientación para tu vestuario
          </p>
          <button
            class="w-[85%] bg-tertiary text-white uppercase rounded-full font-bold px-6 py-4 text-[15px]"
            on:click={() => (isOpenDressModal = true)}>Ver Más</button
          >
        </div>
      </div>

      <div class="mt-14 px-8 w-[420px]">
        <div
          class="px-6 py-12 bg-[#f5f5f5] shadow-lg rounded-2xl min-h-[400px] flex flex-col justify-between items-center"
        >
          <h3 class="font-bold text-primary text-2xl mb-2">
            Confirmar asistencia
          </h3>
          <img
            class="w-auto h-[70px] mb-4"
            src={infoIcon}
            alt="Confirmar asistencia"
            loading="lazy"
          />
          <p class="text-secondary font-normal">
            Confirma tu asistencia a la fiesta
          </p>
          <a
            href="https://wa.me/5491170165805?text=Hola%20Ro!%20Queremos%20confirmarte%20nuestra%20asistencia%20a%20tu%20boda,%20estamos%20contentos%20de%20poder%20pasar%20este%20hermoso%20momento%20con%20ustedes..."
            target="_blank"
            rel="noopener noreferrer"
            class="w-[85%] bg-tertiary text-white uppercase rounded-full font-bold px-6 py-4 text-[15px]"
            >Confirmar</a
          >
        </div>
      </div>
    </div>
  </div>
</section>

{#if isOpenDressModal}
  <DressModal bind:isOpen={isOpenDressModal} />
{/if}
