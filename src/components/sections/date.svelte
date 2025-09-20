<script lang="ts">
  import linesIMG from "../../assets/img/lines01.svg";
  import cintaLIMG from "../../assets/img/cinta01.svg";
  import cintaRIMG from "../../assets/img/cinta02.svg";
  import loveIcon from "../../assets/icons/love.gif";
  import confettiIcon from "../../assets/icons/confetti.gif";
  import grupo02aIMG from "../../assets/img/Grupo02_a.png";
  import grupo02bIMG from "../../assets/img/Grupo02_b.png";
  import grupo02cIMG from "../../assets/img/Grupo02_c.png";
</script>

<section
  class="relative pb-[20%] bg-center bg-no-repeat flex items-center justify-center bg-white pt-30"
  style="background-image: url({linesIMG})"
>
  <img
    src={linesIMG}
    alt="Decorative lines"
    class="absolute top-0 left-0 w-full h-auto mt-30"
  />

  <img
    class="absolute w-[200px] h-auto top-[280px] -left-[30px]"
    src={grupo02aIMG}
    alt=""
    loading="lazy"
  />

  <img
    class="absolute w-[200px] h-auto top-[280px] -left-[30px]"
    src={grupo02bIMG}
    alt=""
    loading="lazy"
  />

  <img
    class="absolute w-[200px] h-auto top-[280px] -left-[30px]"
    src={grupo02cIMG}
    alt=""
    loading="lazy"
  />

  <div
    class="flex flex-wrap px-6 md:px-24 w-full z-10 content-center justify-center"
  >

    <div
      class="text-center flex flex-col items-center justify-center w-[100%] md:w-[50%]"
    >
      <div
        class="w-[175px] h-[175px] mx-5 bg-[#f5f5f5] rounded-full flex items-center justify-center p-5 shadow-xl"
      >
        <img src={confettiIcon} class="w-[100px] h-auto" alt="Confetti icon" />
      </div>

      <h3
        class="font-heading text-white bg-secondary border-y-4 border-secondary inline-block relative font-normal text-5xl min-w-[60%] mt-8"
      >
        <img
          src={cintaLIMG}
          class="absolute top-0 -left-[15px] h-full w-4"
          alt=""
        />
        Fiesta
        <img
          src={cintaRIMG}
          class="absolute top-0 -right-[15px] h-full w-4"
          alt=""
        />
      </h3>

      <div class="mt-8">
        <div class="mb-12">
          <h6 class="font-bold text-secondary text-2xl mb-2">Día</h6>
          <p class="font-normal text-secondary text-xl mb-4">
            Sábado 29 de Noviembre - 18:20 hs
          </p>
          <a
            href="https://calendar.app.google/dRhUE5PjBmqTTqEj8"
            target="_blank"
            rel="noopener noreferrer"
            class="mt-1 inline-block bg-tertiary text-white font-bold py-2 px-12 rounded-full uppercase"
            tabindex="0"
          >
            Agendar
          </a>
        </div>

        <div class="mb-12">
          <h6 class="font-bold text-secondary text-2xl mb-2">Lugar</h6>
          <p class="font-normal text-secondary text-xl mb-4">
            Quinta San José Eventos
          </p>
          <a
            href="https://wa.me/5491170165805?text=Hola%20Ro!%20Queremos%20confirmarte%20nuestra%20asistencia%20a%20tu%20boda,%20estamos%20contentos%20de%20poder%20pasar%20este%20hermoso%20momento%20con%20ustedes..."
            target="_blank"
            rel="noopener noreferrer"
            class="mt-1 inline-block bg-tertiary text-white font-bold py-2 px-12 rounded-full uppercase"
            tabindex="0"
          >
            Confirmar asistencia
          </a>
        </div>

        <div class="mb-12">
          <h6 class="font-bold text-secondary text-2xl mb-2">Dirección</h6>
          <p class="font-normal text-secondary text-xl mb-4">
            Calle 361 1573 - Ranelagh
          </p>
          <a
            href="https://maps.app.goo.gl/RcZny9wHSzPhq5CH9"
            class="mt-1 inline-block bg-tertiary text-white font-bold py-2 px-12 rounded-full uppercase"
            tabindex="0"
          >
            ¿Cómo llegar?
          </a>
        </div>
      </div>
    </div>
  </div>
</section>
