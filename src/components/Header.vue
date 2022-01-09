<template>
    <header>
        <div class="logo">
            <img src="../assets/img/logo-small.svg" alt="">
        </div>
    </header>
</template>

<script>
export default {
    name: "App",
    components: {
        
    },
};
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
.logo{
    padding: 15px;
    img{
        width: 50px;
    }
}
header{
    background-color: $color_header;
}
</style>
