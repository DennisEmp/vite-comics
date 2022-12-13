<script>
    export default{
        data(){
            return {
                icons: [
                    {
                        icon: '/public/img/buy-comics-digital-comics.png',
                        text: 'DIGITAL COMICS',
                    },
                    {
                        icon: '/public/img/buy-comics-merchandise.png',
                        text: 'DC MERCHANDISE',
                    },
                    {
                        icon: '/public/img/buy-comics-subscriptions.png',
                        text: 'SUBSCRIPTION',
                    },
                    {
                        icon: '/public/img/buy-comics-shop-locator.png',
                        text: 'COMIC SHOP LOCATOR',
                    },
                    {
                        icon: '/public/img/buy-dc-power-visa.svg',
                        text: 'DC  POWER VISA',
                    },
                ]
            }
        }
    }
</script>

<template>
    <div class="container-icon">
        <div v-for="(icon, index) in icons" :key="index" class="container-TopFooter">
            <img :src="icon.icon" alt="">
            <h2 class="testo-icon"> {{ icon.text }} </h2>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/mixins.scss' as *;
@use '../styles/partials/variables' as *;

.container-icon{
    display: flex;
    justify-content: space-between;
    padding-top: 60px;
}
.container-TopFooter {
    display: flex;
    text-align: center;
    font-size: 10px;
    
}

.testo-icon{
    color: #fff;
    margin-top: 30px;
    margin-left: 15px;
}

img {
    width: 60px;
    height: 70px;
}
</style>