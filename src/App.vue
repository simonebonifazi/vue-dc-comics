<template>
  <div class="bg">
    <MyHeader :links="links" />
    <MainContent :cards="cards" />
    <FooterTop :links="links" :dcLinks="dcLinks" :sitesLinks="sitesLinks" />
    <FooterBottom :images="images" />
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MainContent from './components/MainContent.vue'
import FooterTop from './components/FooterTop.vue'
import FooterBottom from './components/FooterBottom.vue'

export default {
  name: 'dc-comics',
  components: {
    MyHeader,
    MainContent,
    FooterTop,
    FooterBottom,
  },
      data(){
        return{
           cards: [
        {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
            "price": "$19.99",
            "series": "Action Comics",
            "type": "comic book"
        },
        {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
            "price": "$3.99",
            "series": "American Vampire 1976",
            "type": "comic book"
        },
        {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
            "price": "$16.99",
            "series": "Aquaman",
            "type": "graphic novel"
        },
        {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
            "price": "$2.99",
            "series": "Batgirl",
            "type": "comic book"
        },
        {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
            "price": "$3.99",
            "series": "Batman",
            "type": "comic book"
        },
        {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
            "price": "$2.99",
            "series": "Batman Beyond",
            "type": "comic book"
        },
        {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
            "price": "$3.99",
            "series": "Batman/Superman",
            "type": "comic book"
        },
        {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
            "price": "$4.99",
            "series": "Batman/Superman Annual",
            "type": "comic book"
        },
        {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
            "price": "$5.99",
            "series": "Batman: The Joker War Zone",
            "type": "comic book"
        },
        {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
            "price": "$6.99",
            "series": "Batman: Three Jokers",
            "type": "comic book"
        },
        {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
            "price": "$4.99",
            "series": "Batman: White Knight Presents: Harley Quinn",
            "type": "comic book"
        },
        {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
            "price": "$16.99",
            "series": "Catwoman",
            "type": "graphic novel"
        }
            ],
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
        {
          text: 'Shop',
          url: '#',
          current: false,
        },
            ],
          images: [
      {
            id: 1,
            url: "#",
            src: require("./assets/img/footer-facebook.png"),
            alt: "facebook logo"
        },
        {
            id: 2,
            url: "#",
            src: require("./assets/img/footer-twitter.png"),
            alt: "twitter logo"
        },
        {
            id: 3,
            url: "#",
            src: require("./assets/img/footer-youtube.png"),
            alt: "youtube logo"
        },
        {
            id: 4,
            url: "#",
            src: require("./assets/img/footer-pinterest.png"),
            alt: "pinterest logo"
        },
        {
            id: 5,
            url: "#",
            src: require("./assets/img/footer-periscope.png"),
            alt: "periscope logo"
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

<style lang="scss">
@import "./assets/sass/style.scss";
</style>
