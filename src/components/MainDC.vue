<template>
  <main>
      <div class="container">
          Contents goes here
      </div>
  </main>
</template>

<script>

export default {
    name: 'MainDC',
    data () {
        return {
        }
    }
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/variables.scss';

main{
    background-color: $darkGray;
    .container{
        height: 200px;
        display: flex;
        align-items: center;
        color: white;
        font-weight: 500;
    }
}


</style>