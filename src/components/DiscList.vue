<template>
    <main>
        <div class="conatainer">
            <Filter />
        </div>

        <div class="container">
            <DiscCard v-for="(element, index) in disc.response" :key="index" />
            <DiscCard v-for="(element, index) in disc.response" :key="index" :details="element" />
        </div>
    </main>
</template>

<script>
import axios from 'axios';

import DiscCard from './DiscCard';
import Filter from './Filter';

export default {
    nome: 'DiscList',
    components: {
        DiscCard,
        Filter,
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