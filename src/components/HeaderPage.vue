<template>
  <header>
    <div class="navbar">
      <img
        src="@/img/dc-logo.png"
        alt="logo"
      >
      <ul class="menu-list">
        <li
          v-for="element in arrNavbar"
          :key="element.text"
        >
          <a :href="element.url">{{ element.text }}</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderPage',
  data() {
    return {
      arrNavbar: [
        {
          url: '#characters',
          text: 'characters',
        },
        {
          url: '#comics',
          text: 'comics',
        },
        {
          url: '#movies',
          text: 'movies',
        },
        {
          url: '#tv',
          text: 'tv',
        },
        {
          url: '#games',
          text: 'games',
        },
        {
          url: '#collectibles',
          text: 'collectibles',
        },
        {
          url: '#videos',
          text: 'videos',
        },
        {
          url: '#fans',
          text: 'fans',
        },
        {
          url: '#news',
          text: 'news',
        },
        {
          url: '#shop',
          text: 'shop',
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
$brand_color: rgb(12, 124, 236);

header{
  height: 100px;
}

.navbar{
  display: flex;
  max-width: 1200px;
  margin: auto;
  justify-content: space-between;
  align-items: center;
  height: 100%;

  img{
    width: 70px;
  }

  .menu-list{
    display: flex;
    list-style: none;
    height: 100%;

    li{
      display: flex;
      align-items: center;
      height: 100%;
      margin-left: 1.5rem;
      font-size: 15px;
      font-weight: 700;
      text-transform: uppercase;
      cursor: pointer;

      a{
        text-decoration: none;
        color: rgb(76, 70, 70);
      }

      &:hover{
        border-bottom: 3px solid $brand_color;
      }

      &:hover a{
        color: $brand_color;
      }
    }
  }
}

</style>
