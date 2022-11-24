<template>
  <main>
    <div class="container">
      -- Content Here --
    </div>
  </main>
</template>

<script>
export default {
  name: 'ContentPage',
};
</script>

<style lang="scss" scoped>
  main{
    background-color: black;
    color: white;
    font-size: 20px;

    .container{
      height: 100px;
      max-width: 1200px;
      display: flex;
      align-items: center;
      margin: 0 auto;
    }
  }
</style>
