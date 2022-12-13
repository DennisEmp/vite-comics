<script>
    export default {
        data() {
            return {

                footerFirstNav: [
                    {
                        text: 'Characters',
                        url: '#',
                    },
                    {
                        text: 'Comics',
                        url: '#',
                    },
                    {
                        text: 'Movies',
                        url: '#',
                    },
                    {
                        text: 'TV',
                        url: '#',
                    },
                    {
                        text: 'Games',
                        url: '#',
                    },
                    {
                        text: 'Videos',
                        url: '#',
                    },
                    {
                        text: 'News',
                        url: '#',
                    }
                ],

                footerSecondNav: [
                    {
                        text: 'Shop DC',
                        url: '#',
                    },
                    {
                        text: 'Shop DC Collectibles',
                        url: '#',
                    },
                ],

                footerThirdNav: [
                    {
                        text: 'Terms of Use',
                        url: '#',
                    },
                    {
                        text: 'Privacy Policy (NEW)',
                        url: '#',
                    },
                    {
                        text: 'Ad Choices',
                        url: '#',
                    },
                    {
                        text: 'Advertising',
                        url: '#',
                    },
                    {
                        text: 'Jobs',
                        url: '#',
                    },
                    {
                        text: 'Subscriptions',
                        url: '#',
                    },
                    {
                        text: 'Talent Workshops',
                        url: '#',
                    },
                    {
                        text: 'CPSC Certificates',
                        url: '#',
                    },
                    {
                        text: 'Ratings',
                        url: '#',
                    },
                    {
                        text: 'Shop Help',
                        url: '#',
                    },
                    {
                        text: 'Contact Us',
                        url: '#',
                    },
                ],

                footerForthNav: [
                    {
                        text: 'DC',
                        url: '#',
                    },
                    {
                        text: 'MAD Magazine',
                        url: '#',
                    },
                    {
                        text: 'DC Kids',
                        url: '#',
                    },
                    {
                        text: 'DC Universe',
                        url: '#',
                    },
                    {
                        text: 'DC Power Visa',
                        url: '#',
                    },
                ],
            }
        },
    }
</script>

<template>
    <div class="container-link-2">
        <div class="container-link">
            <h2>DC COMICS</h2>
            <br>
            <ul>
                <li v-for="(link, index) in footerFirstNav" :key="index">
                    <a :href="link.url"> {{ link.text }} </a>
                </li>
            </ul>
            <h2>SHOP</h2>
            <br>
            <ul>
                <li v-for="(link, index) in footerSecondNav" :key="index">
                    <a :href="link.url"> {{ link.text }} </a>
                </li>
            </ul>
            <h2>DC</h2>
            <br>
            <ul>
                <li v-for="(link, index) in footerThirdNav" :key="index">
                    <a :href="link.url"> {{ link.text }} </a>
                </li>
            </ul>
            <h2>SITES</h2>
            <br>
            <ul>
                <li v-for="(link, index) in footerForthNav" :key="index">
                    <a :href="link.url"> {{ link.text }} </a>
                </li>
            </ul>
        </div>
        <div>
            <img src="/public/img/dc-logo-bg.png" alt="">
        </div>
    </div>
    <div class=".container-bottom-footer">
        <div>
            <button>SIGN-UP NOW!</button>
            <h2 class="follow">FOLLOW US</h2>
            <!-- icone social -->
        </div>
    </div>
</template>

<style lang="scss" scoped>
a {
    text-decoration: none;
    color: #7f8883;
}
ul li {
    list-style-type: none;
    width: 150px;
}
ul {
    width: 150px;
}
h2 {
    color: #fff;
    width: 150px;
}
.container-link {
    height: 500px;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    width: 28rem;
    padding-top: 3rem;
}
img {
    position: relative;
    top: -583px;
    left: 795px;
    width: 659px;
}
</style>