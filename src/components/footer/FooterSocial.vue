<script>
export default {
    name: 'FooterSocial',

    data () {
        return {
            social: [
                '/img/footer-facebook.png',
                '/img/footer-twitter.png',
                '/img/footer-youtube.png',
                '/img/footer-pinterest.png',
                '/img/footer-periscope.png'
            ]
        }
    }
}
</script>

<template>
    <div>
        <div class="my_flex my_height3">
            <div>
                <button class="btn_style">sign-up now!</button>
            </div>
            <div class="my_flex my_follow">
                <div class="my_footer_text">
                    follow us
                </div>
                <div v-for="currentImage in social"  class="my_flex my_social">
                    <img :src="currentImage" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss">

    @use '../../style/general.scss' as *;

    .my_height3{
        padding: 45px 0px;
        justify-content: space-between;
        align-items: center;

        .btn_style{
            background-color: #303030;
            text-transform: uppercase;
            font-size: 20px;
            color: white;
            padding: 10px 20px;
            border: 2px solid $primaryColor;
        }

        .my_follow {
            gap: 20px;
            align-items: center;


            .my_footer_text{
                font-size: 20px;
                font-weight: 900;
                text-transform: uppercase;
                color: $primaryColor;
            }

            .my_social {
                width: 40px;
                height: 40px;
            }
        }

    }
</style>