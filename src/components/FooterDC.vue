<template>
  <footer>
      <div class="container">
          <div>
              <ul>
                  <li></li>
              </ul>
          </div>
          <div>
              <img src="../assets/img/dc-logo-bg.png" alt="">
          </div>
      </div>
  </footer>
</template>

<script>
export default {
    name: 'FooterDC',
    data () {
        return {
            sections:[
                {
                    name: 'DC COMICS',
                    subsection:[
                        {text:'Characters'},
                        {text:'Comics'},
                        {text:'Movies'},
                        {text:'TV'},
                        {text:'Games'},
                        {text:'Videos'},
                        {text:'News'}
                    ]
                },
                {
                    name: 'DC SHOP',
                    subsection:[
                        {text:'Shop DC'},
                        {text:'Shop DC Collectibles'}
                    ]
                },
                {
                    name: 'DC',
                    subsection:[
                        {text:'Terms Of Use'},
                        {text:'Privacy Policy (New)'},
                        {text:'Advertising'},
                        {text:'Jobs'},
                        {text:'Subscriptions'},
                        {text:'CPSC Certificates'},
                        {text:'Ratings'},
                        {text:'Shop Help'},
                        {text:'Contact Us'},
                    ]
                },
                {
                    name: 'SITE',
                    subsection:[
                        {text:'DC'},
                        {text:'DC UNIVERSE INFINITE'},
                        {text:'DC Kids'},
                        {text:'DC Shop'},
                        {text:'MAD Magazine'}
                    ]
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">

footer{
    height: 400px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}

img{
    height: 200px;
}

</style>