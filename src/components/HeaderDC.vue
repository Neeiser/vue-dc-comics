<template>
  <header>
      <img src="../assets/img/dc-logo.png" alt="DC Logo">
      <ul>
          <li v-for="(link, index) in categories" :key="index"><a :href="link.href">{{ link.text }}</a></li>
      </ul>
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
li{
    display: inline-block;
    a{
        display: inline-block;
        text-decoration: none;
    }
}
</style>