<script>
export default {
    name: 'AppNav',

    data() {
        return {
            link: [
                'Characters',
                'Comics',
                'Movies',
                'Tv',
                'Games',
                'Collectibles',
                'Videos',
                'Fans',
                'News',
                'Shop'
            ],

            activeContent: 1,
        }
    }
}
</script>


<template>
    <nav class="my_nav">
        <div class="my_width my_width2 my_flex">
            <div>
                <img src="/img/dc-logo.png" alt="dc logo">
            </div>

            <div class="my_flex">
                <ul v-for="(currentLink, index) in link" :class="index == activeContent ? 'active' : ''" class="my_list2">
                    <li>{{ currentLink }}</li>
                </ul>
            </div>
        </div>      
    </nav>
</template>


<style lang="scss">
    .my_nav {
        background-color: white;
        color: black;

        .my_width2{
            display: flex;
            justify-content: space-between;
            align-items: center;

            .active{
                color: #0c7cec;
                border-bottom: 5px solid #0c7cec;
            }

            .my_list2{
                font-weight: bold;
                padding: 50px 15px;
                list-style-type: none;
            }
        }
    }
</style>