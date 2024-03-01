<script>
export default {
    name: 'FooterSocial',

    data () {
        return {
            social: [
                'footer-facebook.png',
                'footer-twitter.png',
                'footer-youtube.png',
                'footer-pinterest.png',
                'footer-periscope.png'
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
                    <img src="../../../public/img/footer-facebook.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
    .my_height3{
        padding: 50px 0px;
        justify-content: space-between;
        align-items: center;

        .btn_style{
            background-color: #303030;
            text-transform: uppercase;
            font-size: 20px;
            color: white;
            padding: 20px;
            border: 2px solid #0282f9;
        }

        .my_follow {
            gap: 20px;
            align-items: center;


            .my_footer_text{
                font-size: 20px;
                font-weight: 900;
                text-transform: uppercase;
                color: #0282f9;
            }

            .my_social {
                width: 40px;
                height: 40px;
            }
        }

    }
</style>