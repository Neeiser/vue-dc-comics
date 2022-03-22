<template>
    <section>
        <div class="container">
            <div class="footer-social-btn">
                <button>SIGN-UP NOW!</button>
            </div>
            <div class="footer-socials">
                <strong>FOLLOW US</strong>
                <a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a>
                <a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a>
                <a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a>
                <a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a>
                <a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'FooterSocialDC',
    data () {
        return {
        }
    }
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/variables.scss';

section *{
    z-index:5;
}

section{
    height: 134px; /* DEBUG */
    background-color: #383838;
}

.container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    .footer-social-btn,
    .footer-socials{
        display: flex;
        align-items: center;
        height: 134px;
    }
}

button {
    color: white;
    font-weight: 600;
    padding: 15px;
    background-color: transparent;
    border: 3px solid $blueDC;
}

button:active {
    color: white;
    font-weight: 600;
    padding: 15px;
    background-color: transparent;
    border: 3px solid $activeBlueDC;
}

.footer-socials *{
    padding: 0 5px;
}

strong{
    font-size: 1.5rem;
    color: $blueDC;
}

</style>