<template>
    <main>
        <div class="container containerShowcase">
            <h1>CURRENT SERIES</h1>
            <div class="gridDC">
                <GridShowcaseDC v-for="card in arrComics" :key="card.series"
                :comic-img="card.thumb"
                :comic-series="card.series"
                >
                </GridShowcaseDC>
            </div>
            <button>LOAD MORE</button>
        </div>
    </main>
</template>

<script>
import GridShowcaseDC from './GridShowcaseDC.vue'

export default {
    name: 'MainDC',
    data () {
        return {
            arrComics:[
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    price: "$19.99",
                    series: "Action Comics",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    price: "$3.99",
                    series: "American Vampire 1976",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    price: "$16.99",
                    series: "Aquaman",
                    type: "graphic novel"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    price: "$2.99",
                    series: "Batgirl",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    price: "$3.99",
                    series: "Batman",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    price: "$2.99",
                    series: "Batman Beyond",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    price: "$3.99",
                    series: "Batman/Superman",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    price: "$4.99",
                    series: "Batman/Superman Annual",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    price: "$5.99",
                    series: "Batman: The Joker War Zone",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    price: "$6.99",
                    series: "Batman: Three Jokers",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    price: "$4.99",
                    series: "Batman: White Knight Presents: Harley Quinn",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    price: "$16.99",
                    series: "Catwoman",
                    type: "graphic novel"
                }
            ]
        }
    },
    components: {
        GridShowcaseDC
    }
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/variables.scss';

main{
    background-color: $darkGray;
    .gridDC{
        display: flex;
        align-items: stretch;
        flex-wrap: wrap;
        justify-content: center;
        color: white;
        font-weight: 500;
        padding: 50px 0;
    }
}
.containerShowcase{
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    padding-bottom: 50px;
    position: relative;
    h1{
        background-color: $blueDC;
        color: white;
        padding: 10px 40px;
        position: absolute;
        top: -30px;
        left: 0;
    }
    button{
        color: white;
        background-color: $blueDC;
        border: none;
        padding: 10px 40px;
    }
    
    button:active{
        background-color: $activeBlueDC;
        padding: 10px 35px;
        transition: 0.1s;
    }
}


</style>