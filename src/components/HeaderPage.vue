<template>
  <header>
    <div class="navbar">
      <img src="@/img/dc-logo.png" alt="logo">
      <ul class="menu-list">
        <li>Characters</li>
        <li class="active">Comics</li>
        <li>Movies</li>
        <li>TV</li>
        <li>Games</li>
        <li>Collectibles</li>
        <li>Videos</li>
        <li>Fans</li>
        <li>News</li>
        <li>Shop</li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderPage',
};
</script>

<style lang="scss" scoped>
$brand_color: rgb(12, 124, 236);

header{
  height: 100px;
  padding: 1rem 0;
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
      color: rgb(76, 70, 70);
      cursor: pointer;

      &:hover{
        color: $brand_color;
        border-bottom: 3px solid $brand_color;
      }
    }

    .active{
      color: $brand_color;
      border-bottom: 3px solid $brand_color;
    }
  }
}

</style>
