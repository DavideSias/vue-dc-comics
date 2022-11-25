<template>
  <div class="card">
    <div class="main-content">
      <img
        :src="comics.thumb"
        :alt="comics.series"
      >
      <h2>{{ comics.series }}</h2>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardComics',
  props: {
    comics: Object,
  },
};
</script>

<style lang="scss" scoped>

  .main-content{
    height: 100%;
    padding: 1rem 0;

    img{
      max-width: 100%;
      aspect-ratio: 1 / 1;
      object-fit: cover;
      object-position: top;
    }

    h2{
      margin-top: 1rem;
      font-size: 13px;
      font-weight: 400;
      text-transform: uppercase;
    }
  }

</style>
