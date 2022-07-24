<template>
    <div class="footer-top">
        <div class="container d-flex">
            <ul id="main-links" class="d-flex">
                <li class="dc-comics">
                    <h3> DC-COMICS</h3>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                </li>
                <li class="shop">
                    <h3>SHOP</h3>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </li>
                <li class="dc">
                    <h3>DC</h3>
                    <ul>
                        <li>Terms Of Use</li>
                        <li>Privacy policy (New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscription</li>
                        <li>Talent Workshop</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings </li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </li>
                <li class="sites">
                    <h3>SITES</h3>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </li>
            </ul>
            <figure>
                <img id="big-logo" src="../assets/img/dc-logo-bg.png" alt="logo-big">
            </figure>
        </div>
    </div>
</template>

<script>
export default {
    name: "FooterTop"
}
</script>

<style scoped>
.footer-top {
    background-image: url(../assets/img/footer-bg.jpg);

    height: 320px;
}

.container {
    height: 100%;

    justify-content: space-between;
}

#big-logo {
    height: 80%;
}

#main-links {
    color: #fff;
}

h3 {
    margin: 5px 0;
}

.dc-comics li,
.dc li,
.shop li,
.sites li {
    font-size: 12px;
}
</style>