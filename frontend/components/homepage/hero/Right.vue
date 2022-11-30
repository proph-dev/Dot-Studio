<template>
  <div>
    <img src="../../../assets/img/dot-studio-hero.svg" alt="Icône DOT.Studio">
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
  img {
    width: 40rem;
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