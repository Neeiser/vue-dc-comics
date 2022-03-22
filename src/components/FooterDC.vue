<template>
  <footer>
      <div class="container">
          <div>
              <ul v-for="item in sections" :key="item">
                  <strong>{{item.name}}</strong>
              </ul>
                  <li v-for="(subItem, subIndex) in sections[element].subsection" :key="subIndex">
                      <a :href="subItem.href">{{subItem.text}}</a>
                  </li>
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
            element: 0,
            sections:[
                {
                    name: 'DC COMICS',
                    subsection:[
                        {href:'#', text:'Characters'},
                        {href:'#', text:'Comics'},
                        {href:'#', text:'Movies'},
                        {href:'#', text:'TV'},
                        {href:'#', text:'Games'},
                        {href:'#', text:'Videos'},
                        {href:'#', text:'News'}
                    ]
                },
                {
                    name: 'DC SHOP',
                    subsection:[
                        {href:'#', text:'Shop DC'},
                        {href:'#', text:'Shop DC Collectibles'}
                    ]
                },
                {
                    name: 'DC',
                    subsection:[
                        {href:'#', text:'Terms Of Use'},
                        {href:'#', text:'Privacy Policy (New)'},
                        {href:'#', text:'Advertising'},
                        {href:'#', text:'Jobs'},
                        {href:'#', text:'Subscriptions'},
                        {href:'#', text:'CPSC Certificates'},
                        {href:'#', text:'Ratings'},
                        {href:'#', text:'Shop Help'},
                        {href:'#', text:'Contact Us'},
                    ]
                },
                {
                    name: 'SITE',
                    subsection:[
                        {href:'#', text:'DC'},
                        {href:'#', text:'DC UNIVERSE INFINITE'},
                        {href:'#', text:'DC Kids'},
                        {href:'#', text:'DC Shop'},
                        {href:'#', text:'MAD Magazine'}
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