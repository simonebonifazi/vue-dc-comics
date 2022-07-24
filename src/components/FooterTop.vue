<template>
    <div class="footer-top">
        <div class="container d-flex">
            <ul id="main-links" class="d-flex">
                <li class="dc-comics">
                    <h3> DC-COMICS</h3>
                    <ul>
                        <li> <a href="#"> Characters </a></li>
                        <li> <a href="#"> Comics </a></li>
                        <li> <a href="#"> Movies </a></li>
                        <li> <a href="#"> TV </a></li>
                        <li> <a href="#"> Games </a></li>
                        <li> <a href="#"> Videos </a></li>
                        <li> <a href="#"> News </a></li>
                        <li class="shop">
                            <h3>SHOP</h3>
                        </li>
                        <li> <a href="#"> Shop DC </a></li>
                        <li> <a href="#"> Shop DC Collectibles </a></li>
                    </ul>
                </li>
                <li class="dc">
                    <h3>DC</h3>
                    <ul>
                        <li> <a href="#"> Terms Of Use </a></li>
                        <li> <a href="#"> Privacy policy (New) </a></li>
                        <li> <a href="#"> Ad Choices </a></li>
                        <li> <a href="#"> Advertising </a></li>
                        <li> <a href="#"> Jobs </a></li>
                        <li> <a href="#"> Subscription </a></li>
                        <li> <a href="#"> Talent Workshop </a></li>
                        <li> <a href="#"> CPSC Certificates </a></li>
                        <li> <a href="#"> Ratings </a></li>
                        <li> <a href="#"> Shop Help </a></li>
                        <li> <a href="#"> Contact Us </a></li>
                    </ul>
                </li>
                <li class="sites">
                    <h3>SITES</h3>
                    <ul>
                        <li> <a href="#"> DC </a></li>
                        <li> <a href="#"> MAD Magazine </a></li>
                        <li> <a href="#"> DC Kids </a></li>
                        <li> <a href="#"> DC Universe </a></li>
                        <li> <a href="#"> DC Power Visa </a></li>
                    </ul>
                </li>
            </ul>
            <div class="dc-big-logo">
                <!-- <img id="big-logo" src="../assets/img/dc-logo-bg.png" alt="logo-big"> -->
            </div>
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

.dc-big-logo {
    height: 100%;
    width: 100%;
    background-repeat: no-repeat;
    background-position: right;
    background-image: url(../assets/img/dc-logo-bg.png);
}

.container {
    height: 100%;

    justify-content: space-between;
    align-items: center;
}

#big-logo {
    height: 70%;
}

#main-links,
#main-links .shop {
    color: #fff;
    font-size: 16px;

}

h3 {
    margin: 5px 0;
}

.dc-comics li,
.dc li,
.shop li,
.sites li {
    font-size: 12px;
    margin-top: 2px;
    color: #646464
}

.sites,
.dc {
    margin-left: 32px;
}
</style>