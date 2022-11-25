<template>
  <main>
    <div class="container">
      <div class="flex-container">
        <CardComics
          v-for="objComic in arrComics"
          :key="objComic.series"
          class="card-comic"
          :comics="objComic"
        />
      </div>
      <div class="current-series">
        current series
      </div>
      <div class="buttons">
        <button class="load">
          load more
        </button>
      </div>
    </div>
  </main>
</template>

<script>
import CardComics from '@/components/CardComics.vue';

export default {
  name: 'ContentPage',
  components: {
    CardComics,
  },
  data() {
    return {
      arrComics: [
        {
          thumb:
            'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX',
          price: '$19.99',
          series: 'Action Comics',
          type: 'comic book',
        },
        {
          thumb:
            'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01',
          price: '$3.99',
          series: 'American Vampire 1976',
          type: 'comic book',
        },
        {
          thumb:
            'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb',
          price: '$16.99',
          series: 'Aquaman',
          type: 'graphic novel',
        },
        {
          thumb:
            'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76',
          price: '$2.99',
          series: 'Batgirl',
          type: 'comic book',
        },
        {
          thumb:
            'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
          price: '$3.99',
          series: 'Batman',
          type: 'comic book',
        },
        {
          thumb:
            'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
          price: '$2.99',
          series: 'Batman Beyond',
          type: 'comic book',
        },
        {
          thumb:
            'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8',
          price: '$3.99',
          series: 'Batman/Superman',
          type: 'comic book',
        },
        {
          thumb:
            'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk',
          price: '$4.99',
          series: 'Batman/Superman Annual',
          type: 'comic book',
        },
        {
          thumb:
            'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8',
          price: '$5.99',
          series: 'Batman: The Joker War Zone',
          type: 'comic book',
        },
        {
          thumb:
            'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY',
          price: '$6.99',
          series: 'Batman: Three Jokers',
          type: 'comic book',
        },
        {
          thumb:
            'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX',
          price: '$4.99',
          series: 'Batman: White Knight Presents: Harley Quinn',
          type: 'comic book',
        },
        {
          thumb:
            'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq',
          price: '$16.99',
          series: 'Catwoman',
          type: 'graphic novel',
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
$brand_color: rgb(12, 124, 236);
main {
  background-color: rgb(28, 28, 28);
  color: white;
  font-size: 20px;

  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 1.5rem 0;
    position: relative;

    .flex-container{
      display: flex;
      flex-wrap: wrap;
      justify-content: space-around;
    }
    .current-series{
      background-color: $brand_color;
      position: absolute;
      left: 0;
      top: -1rem;
      padding: 0.5rem 1rem;
      font-size: 15px;
      font-weight: 700;
      text-transform: uppercase;
    }

    .buttons{
      margin-top: 2rem;
      text-align: center;
      .load{
        background-color: $brand_color;
        color: white;
        padding: 0.5rem 3rem;
        font-size: 12px;
        font-weight: 700;
        border: none;
        text-transform: uppercase;
        cursor: pointer;

        &:hover{
          background-color: white;
          color: $brand_color;
        }
      }
    }

  }

  .card-comic{
    flex: 0 0 15%;
  }

}
</style>
