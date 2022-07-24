<template>
    <div class="footer-bottom">

        <div class="container d-flex">
            <span>
                <a href="#">SING-UP NOW!</a>
            </span>

            <div class="social-references d-flex">
                <ul class="d-flex">
                    <li>
                        <h3> FOLLOW US </h3>
                    </li>
                    <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook logo"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter logo"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-youtube.png" alt="youtube logo"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest logo"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="periscope logo"></a></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "FooterBottom"
}
</script>

<style scoped>
.footer-bottom {
    background-color: #303030;
    margin-bottom: 15px;
}

.container {
    justify-content: space-between;
    align-items: center;

    padding: 25px;
}

.container span {
    border: 2px solid #0282F9;
    padding: 7px;

    color: #fff;
}

.social-references,
.social-references ul {
    align-items: center;
}

.social-references ul li {
    margin: 0 10px;
}

.social-references h3 {
    color: #0282F9;

}
</style>