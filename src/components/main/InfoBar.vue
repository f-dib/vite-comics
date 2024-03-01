<script>
export default {
    name: 'InfoBar',

    data (){
        return {
            buy: [
                {
                    img: '/img/buy-comics-digital-comics.png',
                    description: 'Digital Comics'
                },
                {
                    img: '/img/buy-comics-merchandise.png',
                    description: 'Dc Merchandise'
                },
                {
                    img: '/img/buy-comics-shop-locator.png',
                    description: 'Subscription'
                },
                {
                    img: '/img/buy-comics-subscriptions.png',
                    description: 'Comic Shop Locator'
                },
                {
                    img: '/img/buy-dc-power-visa.svg',
                    description: 'Dc Power Visa'
                },
            ]
        }
    }
}
</script>

<template>
    <div>
        <div v-for="currentElement in buy" class="">
                <div class="my_flex_list">
                    <div class="my_img_box"><img class="my_img" :src="currentElement.img" alt=""></div>
                    <div>{{ currentElement.description }}</div>
                </div>
        </div>
    </div>
</template>

<style lang="scss">
    .my_flex_list{
        display: flex;
        align-items: center;
        gap: 15px;

        .my_img_box{
            width: 50px;
            height: 60px;
        }

        .my_img{
            width: 100%;
            height: 100%;
        }
    }
</style>