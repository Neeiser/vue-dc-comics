<template>
  <header>
      <div class="container">
        <img src="../assets/img/dc-logo.png" alt="DC Logo">
        <ul>
            <li v-for="(link, index) in categories" :key="index">
                <a :href="link.href">{{ link.text }}</a>
            </li>
        </ul>
      </div>
  </header>
</template>

<script>
export default {
    name: 'HeaderDC',
    data () {
        return {
            categories:[
                {
                    href: '#',
                    text:'CHARACTERS'
                },
                {
                    href: '#',
                    text:'COMICS'
                },
                {
                    href: '#',
                    text:'MOVIES'
                },
                {
                    href: '#',
                    text:'TV'
                },
                {
                    href: '#',
                    text:'GAMES'
                },
                {
                    href: '#',
                    text:'COLLECTIBLES'
                },
                {
                    href: '#',
                    text:'VIDEOS'
                },
                {
                    href: '#',
                    text:'FANS'
                },
                {
                    href: '#',
                    text:'NEWS'
                },
                {
                    href: '#',
                    text:'SHOP'
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/variables.scss';

.container{
    display: flex;
    align-items: center;
    justify-content: space-between;
}

img{
    height: 80px;
}

li{
    display: inline-block;
    a{
        display: inline-block;
        line-height: 100px;
        padding: 0 15px;
        border-bottom: 3px solid transparent;
        color: $darkGray;
        font-weight: 500;
    };
    a:hover{
        border-bottom: 3px solid $blueDC;
        transition: 0.3s;
    }
}
</style>