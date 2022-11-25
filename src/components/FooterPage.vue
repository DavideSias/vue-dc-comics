<template>
  <footer>
    <div class="footer-links">
      <div class="container">
        <div class="link-list">
          <div class="comics-shop-list">
            <div class="comics-list">
              <ul>
                <h3> DC COMICS </h3>
                <li
                  v-for="element in arrNavbar"
                  :key="element.text"
                >
                  <a :href="element.url">{{ element.text }}</a>
                </li>
              </ul>
            </div>
            <div class="shop-list">
              <ul>
                <h3>SHOP</h3>
                <li
                  v-for="element in arrLinkShop"
                  :key="element.text"
                >
                  <a :href="element.url">{{ element.text }}</a>
                </li>
              </ul>
            </div>
          </div>
          <div class="dc-list">
            <ul>
              <h3> DC </h3>
              <li
                v-for="element in arrLinkDc"
                :key="element.text"
              >
                <a :href="element.url">{{ element.text }}</a>
              </li>
            </ul>
          </div>
          <div class="sites-list">
            <ul>
              <h3> SITES </h3>
              <li
                v-for="element in arrSites"
                :key="element.text"
              >
                <a :href="element.url">{{ element.text }}</a>
              </li>
            </ul>
          </div>
        </div>
        <div
        class="img-container"></div>
      </div>
    </div>
    <div class="footer-social">
      <div class="container">
        <button>SIGN-UP NOW!</button>
        <div class="social">
          <div class="follow-us">
            FOLLOW US
          </div>
          <div class="icons">
            <img
              src="@/img/footer-facebook.png"
              alt="facebook"
            >
            <img
              src="@/img/footer-twitter.png"
              alt="facebook"
            >
            <img
              src="@/img/footer-youtube.png"
              alt="facebook"
            >
            <img
              src="@/img/footer-pinterest.png"
              alt="facebook"
            >
            <img
              src="@/img/footer-periscope.png"
              alt="facebook"
            >
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterPage',
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

      arrLinkShop: [
        {
          url: '#shopdc',
          text: 'shop DC',
        },
        {
          url: '#shopdc-collectibles',
          text: 'shop DC collectibles',
        },
      ],

      arrLinkDc: [
        {
          url: '#terms-of-use',
          text: 'terms of use',
        },
        {
          url: '#privacy',
          text: 'privacy policy (new)',
        },
        {
          url: '#ad',
          text: 'ad choices',
        },
        {
          url: '#adv',
          text: 'advertising',
        },
        {
          url: '#jobs',
          text: 'jobs',
        },
        {
          url: '#subscriptions',
          text: 'subscriptions',
        },
        {
          url: '#talent-workshop',
          text: 'talent workshop',
        },
        {
          url: '#CPSC',
          text: 'CPSC certificate',
        },
        {
          url: '#ratings',
          text: 'ratings',
        },
        {
          url: '#shop-help',
          text: 'shop help',
        },
        {
          url: '#contact-us',
          text: 'contact us',
        },
      ],

      arrSites: [
        {
          url: '#DC',
          text: 'DC',
        },
        {
          url: '#MAD',
          text: 'MAD megazine',
        },
        {
          url: '#DC-kids',
          text: 'DC kids',
        },
        {
          url: '#DC-universe',
          text: 'DC universe',
        },
        {
          url: '#DC-power-visa',
          text: 'DC power visa',
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
$brand_color: rgb(12, 124, 236);
  .footer-links{
    background-image: url('@/img/footer-bg.jpg');
    background-size: cover;

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

          h3{
            margin-bottom: 1rem;
            font-size: 1rem;
          }

          li{
            font-weight: 500;
            margin: .3rem 0;
            font-size: 13px;
            cursor: pointer;

            a{
              text-decoration: none;
              color: gray;
              text-transform: capitalize;

              &:hover{
                text-decoration: underline;
                color: white;
              }
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
        cursor: pointer;

        .follow-us:hover{
          color: white;
          text-decoration: underline;
        }

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
