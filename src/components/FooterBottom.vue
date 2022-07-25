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
                    <!-- <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook logo"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter logo"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-youtube.png" alt="youtube logo"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest logo"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="periscope logo"></a></li> -->
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "FooterBottom",
    data() {
        return {
            images: [
                {
                    id: 1,
                    url: "#",
                    src: require("../assets/img/footer-facebook.png"),
                    alt: "facebook logo"
                },
                {
                    id: 2,
                    url: "#",
                    src: require("../assets/img/footer-twitter.png"),
                    alt: "twitter logo"
                },
                {
                    id: 3,
                    url: "#",
                    src: require("../assets/img/footer-youtube.png"),
                    alt: "youtube logo"
                },
                {
                    id: 4,
                    url: "#",
                    src: require("../assets/img/footer-pinterest.png"),
                    alt: "pinterest logo"
                },
                {
                    id: 5,
                    url: "#",
                    src: require("../assets/img/footer-periscope.png"),
                    alt: "periscope logo"
                },
            ],
        }
    },
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