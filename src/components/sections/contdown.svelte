<script lang="ts">
  import counterIMG from "../../assets/img/contador.png";
  import curvasIMG from "../../assets/img/curvas01.svg";
  import heartIcon from "../../assets/icons/heart.gif";
  import { onMount, onDestroy } from 'svelte';

  const { date } = $props();

  let days = $state(0);
  let hours = $state(0);
  let minutes = $state(0);
  let seconds = $state(0);
  let interval: number;

  function calculateCountdown() {
    const now = new Date().getTime();
    const target = new Date(date).getTime();
    const difference = target - now;

    console.log(difference)

    if (difference > 0) {
      return {
        days: Math.floor(difference / (1000 * 60 * 60 * 24)),
        hours: Math.floor((difference % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60)),
        minutes: Math.floor((difference % (1000 * 60 * 60)) / (1000 * 60)),
        seconds: Math.floor((difference % (1000 * 60)) / 1000)
      };
    } else {
      // Si la fecha ya pasó, mostrar ceros
      return { days: 0, hours: 0, minutes: 0, seconds: 0 };
    }
  }

  function updateCountdown() {
    const result = calculateCountdown();
    days = result.days;
    hours = result.hours;
    minutes = result.minutes;
    seconds = result.seconds;
  }

  onMount(() => {
    updateCountdown(); // Actualizar inmediatamente
    interval = setInterval(updateCountdown, 1000); // Actualizar cada segundo
  });

  onDestroy(() => {
    if (interval) {
      clearInterval(interval);
    }
  });
</script>

<!-- Cuenta regresiva -->
<section class="relative h-80 mt-10 bg-white">
  <img
    class="absolute bg-center -top-[85px] md:-top-[135px] lg:-top-[180px] xl:-top-[220px] z-0 w-full"
    src={curvasIMG}
    alt="Curvas decorativas"
  />
  <div class="flex justify-center align-items-center">
    <div
      class="h-[500px] w-[500px] absolute -ml-9 -top-50 bg-cover flex justify-center align-items-center"
      style="background-image: url({counterIMG})"
    >
      <div class="h-[315px] w-[315px] my-[93px] ml-9 text-center">
        <span
          class="w-full text-center mt-12 text-secondary inline-block text-[40px]"
          >Falta</span
        >

        <div id="reloj" class="mt-2.5 mb-7">
          <div
            id="dias"
            class="w-[25%] py-2 float-left border-r-2 border-[#ccc]"
          >
            <span class="font-bold text-primary inline-block w-full text-4xl"
              >{days}</span
            >
            <span class="text-secondary inline-block w-full font-light text-2xl"
              >{days > 1 ? "días" : "día"}</span
            >
          </div>

          <div
            id="horas"
            class="w-[25%] py-2 float-left border-r-2 border-[#ccc]"
          >
            <span class="font-bold text-primary inline-block w-full text-4xl"
              >{hours}</span
            >
            <span class="text-secondary inline-block w-full font-light text-2xl"
              >hs</span
            >
          </div>

          <div
            id="minutos"
            class="w-[25%] py-2 float-left border-r-2 border-[#ccc]"
          >
            <span class="font-bold text-primary inline-block w-full text-4xl"
              >{minutes}</span
            >
            <span class="text-secondary inline-block w-full font-light text-2xl"
              >min</span
            >
          </div>

          <div id="segundos" class="w-[25%] py-2 float-left no-border">
            <span class="font-bold text-primary inline-block w-full text-4xl"
              >{seconds}</span
            >
            <span class="text-secondary inline-block w-full font-light text-2xl"
              >seg</span
            >
          </div>
        </div>

        <div class="w-full flex justify-center align-items-center">
          <!-- Corazon -->
          <div class="h-14 w-14 relative mt-8">
            <img
              class="absolute inset-0 w-full h-full"
              src={heartIcon}
              alt="Heart icon"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
