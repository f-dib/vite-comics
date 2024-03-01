<script>
import InfoBar from './InfoBar.vue';
import ComicsInfo from './ComicsInfo.vue';

export default {
    name: 'AppContent',

    components: {
        InfoBar,
        ComicsInfo
    },
}
</script>

<template>
    <main>
        <div class="my_content_bg"></div>
        <div class="my_width my_flex_col">
            <div class="buy_area">
                <div></div>
            </div>
            <div><button class="load_more">load more</button></div>
        </div>
    </main>

    <div class="bg">
        <InfoBar class="my_width my_flex my_style"></InfoBar>
    </div>
</template>

<style lang="scss">
        @use '../../style/general.scss' as *;

        .my_content_bg {
            height: 300px;
            background-image: url("../../../public/img/jumbotron.jpg");
            background-size: cover;            
        }
        
        .buy_area{
            padding: 25px 0px;
        }

        .load_more{
            padding: 5px 40px;
            color: white;
            background-color: $primaryColor;
            border: none;
            text-transform: uppercase;
            margin-bottom: 10px;
        }
        
        .bg{
            background-color: $primaryColor;
            padding: 50px 0px;

            .my_style{
                justify-content: space-around;
                align-items: center;
            }
        }
</style>