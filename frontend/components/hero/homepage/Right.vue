<template>
  <div>
    <img src="../../../assets/img/dot-studio-hero.svg" alt="Icône DOT.Studio" class="w-[40rem] max-[1356px]:w-[28rem]">
  </div>
</template>

<style scoped>
  img {
    animation: icon-animation 2s infinite alternate;
  }

  @keyframes icon-animation {
    from {
        -webkit-transform: translate(0);
        transform: translate(0);
    }
    to {
        -webkit-transform: translate(1%, -1%);
        transform: translate(1%, -1%);
    }
  }
</style>