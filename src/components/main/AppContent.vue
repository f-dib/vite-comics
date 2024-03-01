<script>
import InfoBar from './InfoBar.vue';


export default {
    name: 'AppContent',

    components: {
        InfoBar
    },
}
</script>

<template>
    <main class="my_width">
        <div class="my_height">
            -> Content goes Here 
        </div>
    </main>

    <div class="bg">
        <InfoBar class="my_width my_flex my_style"></InfoBar>
    </div>
</template>

<style lang="scss">
    .my_height {
        padding: 50px 5px;
        font-weight: bold;
        font-size: 20px;
    }

   .my_style{
        justify-content: space-around;
        align-items: center;
   }

   .bg{
    background-color: #0c7cec;
    padding: 50px 0px;
   }
</style>