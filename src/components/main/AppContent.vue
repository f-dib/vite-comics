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
    <main>
        <div class="my_width my_height">
            -> Content goes Here 
        </div>
    </main>
    <InfoBar></InfoBar>
</template>

<style lang="scss">
    .my_height {
        padding: 50px 5px;
        font-weight: bold;
        font-size: 20px;
    }
</style>