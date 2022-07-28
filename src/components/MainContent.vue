<template>
    <div class="bg">

        <div class="container">

                <ul class="card-container  d-flex">
                    <MainCard  v-for="(card, i) in cards" :key="i" :card="card" />
                </ul>

        </div>
    </div>
</template>

<script>
import MainCard from './MainCard.vue'
export default {
    name: 'MainContent',
    components: {
        MainCard
    },
    props:{
        cards: Array,
    },
   
}
</script>

<style scoped lang="scss">
.bg {
    color: #fff;
}

.card-container {
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;

    padding: 40px 0;
}
</style>