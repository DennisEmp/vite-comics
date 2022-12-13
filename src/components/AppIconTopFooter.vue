<script>
    export default{
        data(){
            return {
                icons: [
                    {
                        icon: '../assets/img/buy-comics-digital-comics.png',
                        text: 'DIGITAL COMICS',
                    },
                    {
                        icon: '../assets/img/buy-comics-merchandise.png',
                        text: 'DC MERCHANDISE',
                    },
                    {
                        icon: '../assets/img/buy-comics-subscriptions.png',
                        text: 'SUBSCRIPTION',
                    },
                    {
                        icon: '../assets/img/buy-comics-shop-locator.png',
                        text: 'COMIC SHOP LOCATOR',
                    },
                    {
                        icon: '../assets/img/buy-dc-power-visa.svg',
                        text: 'DC  POWER VISA',
                    },
                ]
            }
        }
    }
</script>

<template>
    <div v-for="(icon, index) in icons" :key="index" class="container-TopFooter">
        <img :src="icons.img" alt="">
        <h3> {{ icons.text }} </h3>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/mixins.scss' as *;
@use '../styles/partials/variables' as *;

.container-TopFooter{
    display: flex;
    justify-content: space-between;
}

img {
    width: 30px;
    height: 30px;
}
</style>