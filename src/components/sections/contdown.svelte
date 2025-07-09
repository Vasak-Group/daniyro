<script lang="ts">
  import counterIMG from "../../assets/img/contador.png";
  import curvasIMG from "../../assets/img/curvas01.svg";
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
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 38 32"
              width="38"
              height="32"
              preserveAspectRatio="xMidYMid meet"
              style="width: 100%; height: 100%; transform: translate3d(0px, 0px, 0px);"
              ><defs
                ><clipPath id="__lottie_element_79"
                  ><rect width="38" height="32" x="0" y="0"></rect></clipPath
                ></defs
              ><g clip-path="url(#__lottie_element_79)"
                ><g
                  transform="matrix(0.8683000206947327,0,0,0.8683000206947327,2.5231380462646484,2.049891471862793)"
                  opacity="1"
                  style="display: block;"
                  ><g
                    opacity="1"
                    transform="matrix(1,0,0,1,18.97599983215332,16.06599998474121)"
                    ><path
                      fill="rgb(129,148,139)"
                      fill-opacity="1"
                      d=" M-1.1369999647140503,15.593999862670898 C-0.7720000147819519,15.741999626159668 -0.38600000739097595,15.815999984741211 0.0010000000474974513,15.815999984741211 C0.3869999945163727,15.815999984741211 0.7730000019073486,15.741999626159668 1.1369999647140503,15.593999862670898 C1.8550000190734863,15.300999641418457 18.725000381469727,8.284000396728516 18.725000381469727,-4.073999881744385 C18.725000381469727,-10.550000190734863 13.385000228881836,-15.815999984741211 6.820000171661377,-15.815999984741211 C4.349999904632568,-15.815999984741211 1.9789999723434448,-15.067000389099121 0.0010000000474974513,-13.70199966430664 C-1.9780000448226929,-15.067000389099121 -4.348999977111816,-15.815999984741211 -6.817999839782715,-15.815999984741211 C-13.383999824523926,-15.815999984741211 -18.725000381469727,-10.550000190734863 -18.725000381469727,-4.073999881744385 C-18.725000381469727,8.284000396728516 -1.8550000190734863,15.300999641418457 -1.1369999647140503,15.593999862670898z"
                    ></path></g
                  ></g
                ></g
              ></svg
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
