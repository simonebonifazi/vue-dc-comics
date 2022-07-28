<template>
    <li class="card">
       <figure>
           <a href="#"> <img :src="card.thumb" :alt="card.series"> </a>
        </figure>
        <figcaption v-text="card.series"></figcaption>
    </li>
</template>

<script>
export default {
    name: "MainCard",
    props:{
        card: Object,
    }
    }
</script>

<style scoped lang="scss">
.card{
        flex-basis: calc(100% / 6);
        padding: 10px;
        height: 200px;

        img{
            height: 125px;
            width: 125px;
            object-position: top;
            object-fit: cover;
        }
    }
</style>