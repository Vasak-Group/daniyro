<script lang="ts">
  import counterIMG from "../../assets/img/contador.png";
  import curvasIMG from "../../assets/img/curvas01.svg";
  import heartIcon from "../../assets/icons/heart.gif";
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
              >39</span
            >
            <span class="text-secondary inline-block w-full font-light text-2xl"
              >días</span
            >
          </div>

          <div
            id="horas"
            class="w-[25%] py-2 float-left border-r-2 border-[#ccc]"
          >
            <span class="font-bold text-primary inline-block w-full text-4xl"
              >22</span
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
              >49</span
            >
            <span class="text-secondary inline-block w-full font-light text-2xl"
              >min</span
            >
          </div>

          <div id="segundos" class="w-[25%] py-2 float-left no-border">
            <span class="font-bold text-primary inline-block w-full text-4xl"
              >21</span
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
