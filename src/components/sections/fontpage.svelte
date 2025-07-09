<script lang="ts">

  const date = new Date("2025-11-15");
  const he = "Dani";
  const she = "Rocio";
</script>

<!-- Portada -->
<section class="w-full pb-50 bg-cover relative">
  <picture>
    <source
      type="image/webp"
      srcset="https://fixdate.io/modelo-invitacion/65/img/Grupo01_a.webp"
    />
    <source
      type="image/png"
      srcset="https://fixdate.io/modelo-invitacion/65/img/Grupo01_a.png"
    />
    <img
      class="absolute w-90 h-auto -top-22 left-0 right-0 mx-auto z-[1]"
      src="https://fixdate.io/modelo-invitacion/65/img/Grupo01_a.png"
      alt=""
      loading="lazy"
    />
  </picture>

  <picture>
    <source
      type="image/webp"
      srcset="https://fixdate.io/modelo-invitacion/65/img/Grupo01_b.webp"
    />
    <source
      type="image/png"
      srcset="https://fixdate.io/modelo-invitacion/65/img/Grupo01_b.png"
    />
    <img
      class="absolute w-90 h-auto -top-22 left-0 right-0 mx-auto z-[2]"
      src="https://fixdate.io/modelo-invitacion/65/img/Grupo01_b.png"
      alt=""
      loading="lazy"
    />
  </picture>

  <picture>
    <source
      type="image/webp"
      srcset="https://fixdate.io/modelo-invitacion/65/img/Grupo01_c.webp"
    />
    <source
      type="image/png"
      srcset="https://fixdate.io/modelo-invitacion/65/img/Grupo01_c.png"
    />
    <img
      class="absolute w-90 h-auto -top-22 left-0 right-0 mx-auto"
      src="https://fixdate.io/modelo-invitacion/65/img/Grupo01_c.png"
      alt=""
      loading="lazy"
    />
  </picture>

  <div class="flex justify-center align-items-center">
    <div class="relative z-[999] w-[75%] text-center">
      <div class="pt-44">
        <span
          class="text-primary table no-wrap w-full font-light text-2xl before:content-[''] before:relative before:left-[20%] before:border-t-[1px] before:w-[15%] before:top-[0.9em] before:table-cell after:content-[''] after:border-t-[1px] after:relative after:right-[20%] after:w-[15%] after:top-[0.9em] after:table-cell"
        >
          {date.getDate()}.{date.getMonth() + 1}.{date.getFullYear()}
        </span>
        <h1
          class="text-primary text-[130px] leading-[110px] font-light mb-0 text-center font-heading"
        >
          {he}
          <span
            class="h-15 w-15 rounded-full bg-primary text-white inline-block text-[40px] font-light leading-[60px]"
            >&amp;</span
          >
          {she}
        </h1>
        <div class="w-[50%] mx-auto mt-6 h-[1px] bg-primary"></div>
      </div>

      <div class="pt-9">
        <p>
          <img
            class="inline-block w-8 h-8 my-2.5"
            src="https://fixdate.io/modelo-invitacion/65/img/comilla-apertura.svg"
            alt=""
          /> <br />

          Todos somos mortales, <br /> hasta el primer beso y la segunda copa de
          vino <br />

          <img
            class="inline-block w-8 h-8 my-2.5"
            src="https://fixdate.io/modelo-invitacion/65/img/comilla-cierre.svg"
            alt=""
          />
        </p>
      </div>
    </div>
  </div>
</section>
