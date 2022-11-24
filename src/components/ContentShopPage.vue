<template>
  <div class="shop-section">
    <div class="container">
      <div class="card">
        <img src="@/img/buy-comics-digital-comics.png" alt="digital-comics">
        <span>digital comics</span>
      </div>
      <div class="card">
        <img src="@/img/buy-comics-merchandise.png" alt="merchandise">
        <span>dc merchandise</span>
      </div>
      <div class="card">
        <img src="@/img/buy-comics-subscriptions.png" alt="subscription">
        <span>subscription</span>
      </div>
      <div class="card">
        <img class="location-img" src="@/img/buy-comics-shop-locator.png" alt="shop-locator">
        <span>comic shop locator</span>
      </div>
      <div class="card">
        <img src="@/img/buy-dc-power-visa.svg" alt="visa">
        <span>dc power visa</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ContentShopPage',
};
</script>

<style lang="scss" scoped>
$brand_color: rgb(12, 124, 236);

  .shop-section{
    background-color: $brand_color;
  }
  .container{
    height: 140px;
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    justify-content: space-around;
    align-items: center;

    .card{
      height: 100%;
      display: flex;
      align-items: center;
      font-size: 14px;
      color: white;
      text-transform: uppercase;
      cursor: pointer;

      &:hover{
        text-decoration: underline;
      }

      img{
        width: 45px;
        margin-right: 1rem;
      }

      .location-img{
        width: 37px;
      }
    }
  }
</style>
