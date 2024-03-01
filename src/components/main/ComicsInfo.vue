<script>
export default {
    name: 'ComicsInfo',

    props: {
        comicImage: String,
        comicName: String
    },

    data() {
    },
}
</script>

<template>
    <div class="comic">
        <div class="comics_size"><img class="img-fluid" :src="comicImage" alt="comicName"></div>
        <h4>{{ comicName }}</h4>
    </div>
</template>

<style>
    .comic{
        width: calc(100% / 6);

        padding: 7px;

        .comics_size{
            width: 90%;
            height: 70%;
            margin-bottom: 15px;
        }

        h4{
            text-transform: uppercase;
            font-style: 10px;
        }
    }
</style>