<template>
    <div class="footer-top">
        <div class="container d-flex">
            <ul id="main-links" class="d-flex">
                <li class="dc-comics">
                    <h3> DC-COMICS</h3>
                    <ul>
                        <li v-for="link in links" :key="link.text"> <a :href="link.url"> {{
                                link.text
                        }}</a></li>
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
                        <li v-for="link in dcLinks" :key="link.id"> <a :href="link.url"> {{
                                link.text
                        }}</a></li>
                    </ul>
                </li>
                <li class="sites">
                    <h3>SITES</h3>
                    <ul>
                        <li v-for="link in sitesLinks" :key="link.id"> <a :href="link.url"> {{
                                link.text
                        }}</a></li>

                    </ul>
                </li>
            </ul>
            <div class="dc-big-logo">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "FooterTop",
 
    props: {
        links: Array,
        dcLinks:Array,
        sitesLinks:Array,
    }
}
</script>

<style scoped lang="scss">
.footer-top {
    background-image: url(../assets/img/footer-bg.jpg);

    height: 320px;

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
}



#main-links,
#main-links .shop {
    color: #fff;
    font-size: 16px;

    h3 {
        margin: 5px 0;
    }
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
    padding-left: 30px;
    width: 155px;
}
</style>