<template>
    <div class="footer-bottom">

        <div class="container d-flex">
            <span>
                <a href="#">SING-UP NOW!</a>
            </span>

            <div class="social-references d-flex">
                <ul class="social-links d-flex">
                    <li>
                        <h3> FOLLOW US </h3>
                    </li>
                    <li v-for="image in images" :key="image.id"> <a :href="image.url"> <img :src="image.src"
                                :alt="image.alt"></a></li>
          
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "FooterBottom",
   props: {
    images: Array,
   }
    
}
</script>

<style scoped lang="scss">
.footer-bottom {
    background-color: #303030;
}

.container {
    justify-content: space-between;
    align-items: center;

    padding: 25px 0;

    span {
        border: 2px solid #0282F9;
        padding: 7px;

        color: #fff;
    }
}


.social-references,
.social-links {
    align-items: center;

    h3 {
        color: #0282F9;
    }

    ul {
        li {
            margin: 0 10px;
        }
    }
}
</style>