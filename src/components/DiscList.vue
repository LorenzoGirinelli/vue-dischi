<template>
    <section>
        <div class="container">
            <DiscCard />
        </div>
    </section>
</template>

<script>
import axios from 'axios';
import DiscCard from './DiscCard';

export default {
    nome: 'DiscList',
    components: {
        DiscCard
    },
    data: function () {
        return {
            disc: [],
        }
    },
    created: function() {
        axios.get('https://flynn.boolean.careers/exercises/api/array/music')
        .then((response) => {
            this.disc = response.data;
        });
    }
}
</script>

<style lang="scss" scoped>

</style>