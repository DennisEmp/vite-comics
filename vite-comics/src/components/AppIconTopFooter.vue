<script>
    export default{
        data(){
            return {
                icons: [
                    {
                        img: '../assets/img/buy-comics-digital-comics.png',
                        url: 'DIGITAL COMICS',
                    },
                    {
                        img: '../assets/img/buy-comics-merchandise.png',
                        url: 'DC MERCHANDISE',
                    },
                    {
                        img: '../assets/img/buy-comics-subscriptions.png',
                        url: 'SUBSCRIPTION',
                    },
                    {
                        img: '../assets/img/buy-comics-shop-locator.png',
                        url: 'COMIC SHOP LOCATOR',
                    },
                    {
                        img: '../assets/img/buy-dc-power-visa.svg',
                        url: 'DC  POWER VISA',
                    },
                ]
            }
        }
    }
</script>

<template>
    <div v-for="(icon, index) in icons" :key="index">
        <img src="{{ icons.img }}" alt="">
        <a href=""> {{ icons.url }} </a>
    </div>
</template>

<style lang="scss" scoped>
</style>