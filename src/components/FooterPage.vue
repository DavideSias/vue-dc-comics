<template>
  <footer>
    <div class="footer-links">
      <div class="container">
        <div class="link-list">
          <div class="comics-shop-list">
            <div class="comics-list">
              <ul>
                DC COMICS
                <li class="first-item-list">Characters</li>
                <li>Comics</li>
                <li>Movies</li>
                <li>TV</li>
                <li>Games</li>
                <li>Videos</li>
                <li>News</li>
              </ul>
            </div>
            <div class="shop-list">
              <ul> SHOP
                <li class="first-item-list">Shop DC</li>
                <li>Shop DC Collectibles</li>
              </ul>
            </div>
          </div>
          <div class="dc-list">
            <ul> DC
              <li class="first-item-list">Terms Of Use</li>
              <li>Privacy Policy (New)</li>
              <li>Ad Choices</li>
              <li>Advertising</li>
              <li>Jobs</li>
              <li>subscriptions</li>
              <li>Talent Workshops</li>
              <li>CPSC Certificates</li>
              <li>Ratings</li>
              <li>Shop Help</li>
              <li>Contact Us</li>
            </ul>
          </div>
          <div class="sites-list">
            <ul> SITES
              <li class="first-item-list">DC</li>
              <li>MAD Megazine</li>
              <li>DC Kids</li>
              <li>DC Universe</li>
              <li>DC Power Visa</li>
            </ul>
          </div>
        </div>
        <div class="img-container"></div>
      </div>
    </div>
    <div class="footer-social">
      <div class="container">
        <button>SIGN-UP NOW!</button>
        <div class="social">
          <div>FOLLOW US</div>
          <div class="icons">
            <img src="@/img/footer-facebook.png" alt="facebook">
            <img src="@/img/footer-twitter.png" alt="facebook">
            <img src="@/img/footer-youtube.png" alt="facebook">
            <img src="@/img/footer-pinterest.png" alt="facebook">
            <img src="@/img/footer-periscope.png" alt="facebook">
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterPage',
};
</script>

<style lang="scss" scoped>
$brand_color: rgb(12, 124, 236);
  .footer-links{
    background-image: url('@/img/footer-bg.jpg');

    .container{
      max-width: 1200px;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;

      .img-container{
        width: 50%;
        background-image: url('@/img/dc-logo-bg.png');
        background-position: center;
        background-repeat: no-repeat;
      }

      .link-list{
        display: flex;
        color: white;
        margin: 2rem 0;

        ul{
          font-weight: 700;
          list-style: none;
          margin: 0 1.5rem 1rem 0;

          li{
            font-weight: 500;
            margin: .3rem 0;
            font-size: 13px;
            color: gray;
            cursor: pointer;

            &:hover{
              text-decoration: underline;
              color: white;
            }
          }

          .first-item-list{
            margin-top: 1rem;
          }
        }

        .shop-list{
          margin-top: 2rem;
        }
      }
    }
  }

  .footer-social{
    height: 100px;
    background-color: rgb(48, 48, 48);

    .container{
      max-width: 1200px;
      height: 100%;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: center;

      .social{
        display: flex;
        align-items: center;
        color: $brand_color;
        font-weight: 700;

        img{
          width: 30px;
          margin-left: 1rem;
        }
      }

      button{
        padding: .7rem;
        color: white;
        background-color: rgb(48, 48, 48);
        border: 2px solid $brand_color;
        cursor: pointer;

        &:hover{
          background-color: $brand_color;
        }
      }
    }
  }

</style>
