<script>
    export default{
        data(){
            return {
                // array lista link topbar header
                links: [
                    {
                        txt: 'CHARACTERS',
                        url: '#',
                    },
                    {
                        txt: 'COMICS',
                        url: '#',
                    },
                    {
                        txt: 'MOVIES',
                        url: '#',
                    },
                    {
                        txt: 'TV',
                        url: '#',
                    },
                    {
                        txt: 'GAMES',
                        url: '#',
                    },
                    {
                        txt: 'COLLECTIBLES',
                        url: '#',
                    },
                    {
                        txt: 'VIDEOS',
                        url: '#',
                    },
                    {
                        txt: 'FANS',
                        url: '#',
                    },
                    {
                        txt: 'NEWS',
                        url: '#',
                    },
                    {
                        txt: 'SHOP',
                        url: '#',
                    },
                ]
            }
        }
    }

</script>

<template>
    <header>
        <div class="top-bar">
            <div class="logo">
                <!-- logo -->
                <a href="/">
                    <img src="../assets/img/dc-logo.png" alt="">
                </a>
            </div>
            <!-- lista header -->
            <div class="container-link">
                <ul class="link">
                    <li v-for="(link, index) in links" :key="index" class="elements">
                        <a href="#" class="list-element"> {{ link.txt }} </a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as*;
@use '../styles/general.scss' as*;
@use '../styles/partials/mixins.scss' as*;

.top-bar {
    display: flex;
    justify-content: space-between;
    text-align: center;
    padding-top: 10px;

}
.link {
    display: flex;
    flex-direction: row;
    gap: 15px;
    list-style-type: none;
}
.list-element {
    text-decoration: none;
    color: black;
    text-align: center;
}
.container-link {
    margin-top: 40px;
}
</style>