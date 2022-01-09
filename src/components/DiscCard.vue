<template>
    <div class="song-conteiner">
        <img :src="details.poster">
        <h2>{{ details.title }}</h2>
        <span>{{ details.author }} {{ details.year }}</span>
    </div>
</template>

<script>
export default {
    name: "DiscCard",
    props: {
        details: Object
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
    .song-conteiner{
        background-color: $color_header;
        width: calc(90% / 5);
        height: 350px;
        margin: 10px;
        padding: 30px;
        text-align: center;
        
        img{
            width: 150px;
        }
        h2{
            margin: 10px 0;
            color: $color_text;
        }
        span{
            color: $color_author;
        }
    }
</style>