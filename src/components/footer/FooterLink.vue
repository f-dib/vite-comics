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
                },
                {
                    title: "Dc",
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

    <FooterSocial></FooterSocial>

</template>

<style lang="scss">

</style>