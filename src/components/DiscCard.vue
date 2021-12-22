<template>
    <div class="card contaier">
        <div>
            <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="">
        </div>

        <div class="disc-name">
            <h2>Nome</h2>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Card'
}
</script>

<style lang="scss" scoped>
.card {
    width: calc(100% / 5);
    background-color: #2e3a46;
    &-image{
        img {
        }
    }

    &-name {
        text-align: center;
    }
}
</style>