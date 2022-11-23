<template>
  <section id="first-section">
    <img src="/Home_Icons/HelloWorld.svg" alt="hello world" class="hero" />
    <div class="icons-layer">
      <img src="/Home_Icons/Cross.svg" alt="cross" class="cross" />
      <img src="/Home_Icons/Fragment.svg" alt="fragment" class="fragment" />
      <img src="/Home_Icons/Circle.svg" alt="circle" class="circle" />
      <img src="/Home_Icons/Rubik.svg" alt="rubik" class="rubik" />
    </div>
  </section>
  <!-- <img
    src="/BG_Patterns/SectionSpace1.svg"
    alt="SectionSpace1"
    class="section-space"
  /> -->
  <!-- <div class="section-space"></div> -->
  <!-- <svg
    viewBox="0 0 1728 699"
    fill="blue"
    preserveAspectRatio="none"
    xmlns="http://www.w3.org/2000/svg"
    class="section-space"
  >
    <path
      d="M0 173C524.96 213.579 828.471 229.7 1728 0V699C1143.32 405.635 697.217 332.549 0 429V173Z"
    />
  </svg> -->
  <svg
    width="1728"
    height="746"
    viewBox="0 0 1728 746"
    preserveAspectRatio="none"
    fill="none"
    class="section-space"
    xmlns="http://www.w3.org/2000/svg"
    xmlns:xlink="http://www.w3.org/1999/xlink"
  >
    <path
      d="M0.616551 186.024L-8 185.358V194V450V459.183L1.09626 457.925C349.202 409.768 634.2 403.994 904.954 446.721C1175.69 489.444 1432.58 580.725 1724.41 727.15L1736 732.965V720V21V10.7004L1726.02 13.2487C1276.48 128.041 976.217 181.318 722.921 200.878C469.657 220.436 263.085 206.312 0.616551 186.024Z"
      fill="url(#pattern0)"
      stroke="black"
      stroke-width="16"
    />
    <defs>
      <pattern
        id="pattern0"
        patternContentUnits="objectBoundingBox"
        width="0.0461806"
        height="0.114163"
      >
        <use
          xlink:href="#SectionSpace1Pattern"
          transform="scale(15.38704e-05 0.000383062)"
        />
      </pattern>
      <svg
        width="300"
        height="300"
        viewBox="0 0 300 300"
        fill="none"
        id="SectionSpace1Pattern"
        xmlns="http://www.w3.org/2000/svg"
      >
          <path d="M300 0H0V300H300V0Z" fill="white" />
          <path d="M0 300H50.38L0 250.38V300Z" fill="black" />
          <path
            d="M50.38 0H0V50.38L250.38 300H300V250.38L50.38 0Z"
            fill="black"
          />
          <path d="M250.38 0L300 50.38V0H250.38Z" fill="black" />
      </svg>
    </defs>
  </svg>
  <div class="section-space"></div>
</template>

<script setup lang="ts"></script>

<style>
/* main {
  z-index: -1;
} */
#first-section {
  height: 640px;
  padding-bottom: 100px;
  position: relative;
  /* margin-top: -2px; */
  background: url(BG_Patterns/Section1.svg) top left / 45px 45px, #fcc969;
  background-blend-mode: soft-light, normal;
  position: relative;

  display: flex;
  justify-content: center;
  align-items: center;
}
.hero {
  width: 370px;
}

/* icons */
.icons-layer {
  z-index: 0;
  pointer-events: none;
  position: absolute;
  display: flex;
  /* height: max-content; */
  background-color: aquamarine;
  justify-content: center;
  align-items: center;
}
.icons-layer img {
  position: absolute;
}
.icons-layer .cross {
  height: 150px;
  bottom: 65px;
  right: 260px;
}
.icons-layer .fragment {
  height: 100px;
  top: 130px;
  right: 320px;
}
.icons-layer .circle {
  height: 120px;
  bottom: 130px;
  left: 200px;
}
.icons-layer .rubik {
  height: 230px;
  bottom: -130px;
  left: 290px;
}
.section-space {
  position: absolute;
  top: 550px;
  height: 400px;
  width: 100vw;
  /* fill: #fff5; */
  /* clip-path: path(
    "M 0 173 C 524.96 213.579 828.471 229.7 1728 0 V 699 C 1143.32 405.635 697.217 332.549 0 429 V 173 Z"
  );
  background: url(/BG_Patterns/SectionSpace1Pattern.svg);
  aspect-ratio: initial; */
}
/* .section-space path {
} */
</style>
