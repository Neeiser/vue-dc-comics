<template>
  <section>
      <div class="container">
          <a v-for="(item,index) in tags" :key="index" :href="item.href">
              <img :src="item.img" alt="">
              <span>{{ item.text }}</span>
          </a>
      </div>
  </section>
</template>

<script>
import buyDigitalComics from "../assets/img/buy-comics-digital-comics.png"
import buyComicsMerchandise from "../assets/img/buy-comics-merchandise.png"
import buyComicsSub from "../assets/img/buy-comics-subscriptions.png"
import buyComicsLocation from "../assets/img/buy-comics-shop-locator.png"
import buyVisaDC from "../assets/img/buy-dc-power-visa.svg"

export default {
    name: 'PreFooterDC',
    data () {
        return {
            tags:[
                {
                    href: '#',
                    img: buyDigitalComics,
                    text: 'DIGITAL COMICS',
                },
                {
                    href: '#',
                    img: buyComicsMerchandise,
                    text: 'DC MERCHANDISE',
                },
                {
                    href: '#',
                    img: buyComicsSub,
                    text: 'SUBSCRIPTION',
                },
                {
                    href: '#',
                    img: buyComicsLocation,
                    text: 'COMIC SHOP LOCATOR',
                },
                {
                    href: '#',
                    img: buyVisaDC,
                    text: 'DC POWER VISA',
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/variables.scss';
section{
    background-color: $blueDC;
    .container{
        height: 150px;
        display: flex;
        align-items: center;
        justify-content: center;
        justify-content: space-around;
        a{
            display: flex;
            align-items: center;
            color: white;
            font-weight: 500;
            padding: 20px;
            border-radius: 20px;
            img{
                height: 50px;
            };
            span{
                margin: 0 10px;
            }
        }
    }
}

section *{
    z-index:2;
}

a:hover{
    background-color: $activeBlueDC;
    transition: 0.3s;
}

a:active{
    img{
        transform: scale(90%);
        transition: 0.05s;
    }
    background-color: $blueDC;
    transition: 0.1s;
}

</style>