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
    data() {
        return {
            links: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
            ],
            dcLinks: [
                {
                    id: 1,
                    text: 'Terms Of Use',
                    url: '#',
                },
                {
                    id: 2,
                    text: 'Privacy policy (New)',
                    url: '#',
                },
                {
                    id: 3,
                    text: 'Ad Choices',
                    url: '#',
                },
                {
                    id: 4,
                    text: 'Advertising',
                    url: '#',
                },
                {
                    id: 5,
                    text: 'Jobs',
                    url: '#',
                },
                {
                    id: 6,
                    text: 'Subscription',
                    url: '#',
                },
                {
                    id: 7,
                    text: 'Talent Workshop',
                    url: '#',
                },
                {
                    id: 8,
                    text: 'CPSC Certificates',
                    url: '#',
                },
                {
                    id: 9,
                    text: 'Ratings',
                    url: '#',
                },
                {
                    id: 10,
                    text: 'Shop Help',
                    url: '#',
                },
                {
                    id: 11,
                    text: 'Contact Us',
                    url: '#',
                },
            ],
            sitesLinks: [
                {
                    id: 1,
                    text: 'DC',
                    url: '#',
                },
                {
                    id: 2,
                    text: 'MAD Magazine',
                    url: '#',
                },
                {
                    id: 3,
                    text: 'DC Kids',
                    url: '#',
                },
                {
                    id: 4,
                    text: 'DC Universe',
                    url: '#',
                },
                {
                    id: 5,
                    text: 'DC Power Visa',
                    url: '#',
                },
            ]
        }
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