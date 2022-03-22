<template>
    <footer>
        <div class="container">
            <div class="footer-list">
                <ul>
                    <strong>DC COMICS</strong>
                    <a href=""><li v-for="item in subTextComics" :key="item">{{item.text}}</li></a>
                </ul>
                <ul>
                    <strong>SHOP</strong>
                    <a href=""><li v-for="item in subTextShop" :key="item">{{item.text}}</li></a>
                </ul>
                <ul>
                    <strong>DC</strong>
                    <a href=""><li v-for="item in subTextDC" :key="item">{{item.text}}</li></a>
                </ul>
                <ul>
                    <strong>SITES</strong>
                    <a href=""><li v-for="item in subTextSites" :key="item">{{item.text}}</li></a>
                </ul>     
            </div>
            <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
  </footer>
</template>

<script>
export default {
    name: 'FooterDC',
    data () {
        return {
            subTextComics:[
                {href:'#', text:'Characters'},
                {href:'#', text:'Comics'},
                {href:'#', text:'Movies'},
                {href:'#', text:'TV'},
                {href:'#', text:'Games'},
                {href:'#', text:'Videos'},
                {href:'#', text:'News'}
            ],
            subTextShop:[
                {href:'#', text:'Shop DC'},
                {href:'#', text:'Shop DC Collectibles'}
            ],
            subTextDC:[
                {href:'#', text:'Terms Of Use'},
                {href:'#', text:'Privacy Policy (New)'},
                {href:'#', text:'Advertising'},
                {href:'#', text:'Jobs'},
                {href:'#', text:'Subscriptions'},
                {href:'#', text:'CPSC Certificates'},
                {href:'#', text:'Ratings'},
                {href:'#', text:'Shop Help'},
                {href:'#', text:'Contact Us'},
            ],
            subTextSites:[
                {href:'#', text:'DC'},
                {href:'#', text:'DC UNIVERSE INFINITE'},
                {href:'#', text:'DC Kids'},
                {href:'#', text:'DC Shop'},
                {href:'#', text:'MAD Magazine'}
            ]                    
        }
    }
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/variables.scss';

footer{
    height: 400px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    .container{
        display: flex;
        position: relative;
    }
}

.footer-list{
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    height: 385px;
    margin-top: 15px;
}

ul{
    color: white;
    padding: 20px;
    strong{
        font-size: 1.3rem;
    }
    li{
        color: $iconGray;
        font-size: 0.8rem;
        padding: 5px 0;
    }
}

img{
    height: 550px;
    position: absolute;
    top: 0;
    right: 0;
    top: -70px;
    right: 75px;
    z-index: 1;
}

.footer-social{
    height: 100px;
    background-color: #464646;
}

</style>