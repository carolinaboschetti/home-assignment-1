
<template>
  <carousel :data="data" :controls="true"></carousel>
</template>

<script>
  export default {
    data() {
      return {
        data: [
          '<div class="example-slide"><img src='src/assets/01.jpg'></div>',
          '<div class="example-slide"><img src='src/assets/02.jpg'></div>',
          '<div class="example-slide"><img src='src/assets/03.jpg'></div>',
          '<div class="example-slide"><img src='src/assets/04.jpg'></div>',
          '<div class="example-slide"><img src='src/assets/05.jpg'></div>',
        ],
      };
    },
  };
</script>

<style>
.example-slide {
    align-items: center;
    display: flex;
    font-size: 1.5rem;
    justify-content: center;
    min-height: 10rem;
  }
</style>