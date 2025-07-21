<script lang="ts">
  import giftIcon from "../../assets/icons/gift.gif";
  import group04IMG from "../../assets/img/Grupo04.png";

  export let isOpen: boolean;
</script>

<div
  id="modalVestuario"
  class="fixed top-0 left-0 z-50 h-full w-full outline-0 overflow-y-auto overflow-x-hidden"
  tabindex="-1"
  style="display: block; padding-right: 10px;"
  aria-modal="true"
  role="dialog"
>
  <div
    class="flex items-center justify-center h-full w-full relative m-2 bg-white/90"
  >
    <img
      class="absolute bottom-0 top-0 left-0 right-0 m-auto w-64 h-auto pb-68"
      src={group04IMG}
      alt=""
      loading="lazy"
    />
    <div
      class="text-secondary bg-white text-center rounded-2xl shadow-xl relative flex flex-col p-3 pb-8 z-50"
    >
      <div class="h-24 flex justify-center items-center">
        <!-- Adornos -->

        <button
          type="button"
          class="absolute -top-4 text-white bg-secondary rounded-full h-10 w-10 flex justify-center items-center right-0"
          data-dismiss="modal"
          aria-label="Close"
          on:click={() => (isOpen = false)}
        >
          <span aria-hidden="true">×</span>
        </button>

        <div
          class="h-31 w-31 p-7 bg-white rounded-full shadow-2xl flex justify-center items-center -top-14 relative"
        >
          <img class="" src={giftIcon} alt="" />
        </div>
      </div>

      <div class="inline-block p-0 w-full text-center">
        <h5 class="text-2xl leading-7 font-bold text-primary px-34">
          Regalos
        </h5>
      </div>

      <div class="relative p-4">
        <p class="pb-2">
          ¡No tenemos lista de regalos! Solo una valija y muchas ganas de <br>
          viajar. Si querés acompañarnos en esta escapada soñada, podés hacerlo <br>
          con una transferencia 💕🌍
        </p>

        <ul class="list-disc list-inside text-left ml-6">
          <li><b>Alias:</b> Daniyro</li>
          <li><b>CBU:</b> 4530000800017240220671t</li>
        </ul>
      </div>
    </div>
  </div>
</div>
