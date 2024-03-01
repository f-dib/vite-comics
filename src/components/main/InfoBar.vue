<script>
export default {
    name: 'InfoBar',

    data (){
        return {
            buy: [
                {
                    img: 'buy-comics-digital-comics.png',
                    description: 'Digital Comics'
                },
                {
                    img: 'buy-comics-merchandise.png',
                    description: 'Dc Merchandise'
                },
                {
                    img: 'buy-comics-shop-locator.png',
                    description: 'Subscription'
                },
                {
                    img: 'buy-comics-subscriptions.png',
                    description: 'Comic Shop Locator'
                },
                {
                    img: 'buy-dc-power-visa.svg',
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
                    <div><img class="my_img" src="../../../public/img/buy-comics-digital-comics.png" alt=""></div>
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

        .my_img{
            height: 60px;
        }
    }
</style>