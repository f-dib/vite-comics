<script>
import FooterSocial from './FooterSocial.vue';


export default {
    name: 'FooterLink',

    components: {
      FooterSocial
    },

    data(){

        return {
            link: [
                {
                    title: "Dc Comics",
                    list: [
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Video',
                        'News'
                    ]
                },
                {
                    title: "Shop",
                    list: [
                        'Shop DC',
                        'Shop DC Collectibles',
                    ]
                }
            ],
            link2: [
                {
                    title: "Dc Comics",
                    list: [
                        'Terms Of Use',
                        'Privacy Policy (New)',
                        'Ad Choise',
                        'Advertising',
                        'Jobs',
                        'Subscriptions',
                        'Talent Workshops',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Help',
                        'Contact Us'
                    ]
                },
                {
                    title: "Sites",
                    list: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa',
                    ]
                },
            ]
        }
    }
}
</script>

<template>
    <footer>
        <div class="my_height2 my_position">
            <div class="my_width">
                <div class="my_flex my_space2">
                    <div>
                        <ul v-for="(currentElement) in link" class="my_list my_space3">
                            <li class="my_style2">{{ currentElement.title }}</li>
                            <li v-for="currentLink in currentElement.list">{{ currentLink }}</li>
                        </ul>
                    </div>
                    <ul v-for="(currentElement2) in link2" class="my_list">
                        <li class="my_style2">{{ currentElement2.title }}</li>
                        <li v-for="currentLink2 in currentElement2.list">{{ currentLink2 }}</li>
                    </ul>
                </div>
            </div>
            <img class="my_logo" src="../../../public/img/dc-logo-bg.png" alt="">
        </div>
        <FooterSocial class="my_width"></FooterSocial>
    </footer>

</template>

<style lang="scss">
    .my_height2{
        padding: 40px 0px 60px;

        background-image: url(../../../public/img/footer-bg.jpg);
        background-size: cover;
    }

    .my_position {
        position: relative;

        overflow: hidden;


        .my_space2{
            gap: 20px;
        }

        .my_space3{
            padding-bottom: 20px;
        }

        .my_style2{
            text-transform: uppercase;
            font-weight: 900;
            font-size: 20px;
            padding-bottom: 20px;
        }

        .my_logo{
            position: absolute;
            top: -15%;
            left: 55%;
        }
    }
</style>