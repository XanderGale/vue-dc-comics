<template>
    <div class="navmain">
        <div class="container">
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <img :src="link.icon" :alt="link.title">
                    <span>{{ link.title }}</span>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Navmain',
    data: function(){
        return{
            links: [
                {
                    title: 'Digital Comics',
                    url: '#',
                    icon: require('../assets/img/buy-comics-digital-comics.png')
                },
                {
                    title: 'DC Merchandise',
                    url: '#',
                    icon: require('../assets/img/buy-comics-merchandise.png')
                },
                {
                    title: 'Subscriptions',
                    url: '#',
                    icon: require('../assets/img/buy-comics-subscriptions.png')
                },
                {
                    title: 'Comic Shop Locator',
                    url: '#',
                    icon: require('../assets/img/buy-comics-shop-locator.png')
                },
                {
                    title: 'DC Power Visa',
                    url: '#',
                    icon: require('../assets/img/buy-dc-power-visa.svg')
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

    .navmain{
        background-color: $brand-main-color;
        color: white;
        .container{
            display: flex;
            flex-flow: row nowrap;
            justify-content: space-between;
            align-items: center;
            ul{
                list-style-type: none;
                display: flex;
                flex-flow: row nowrap;
                justify-content: space-between;
                align-items: center;

                padding: 50px;

                width: 100%;
                li{
                    display: flex;
                    flex-flow: row nowrap;
                    justify-content: center;
                    align-items: center;
                    cursor: pointer;
                    img{
                        max-height: 60px;
                        width: 50px;
                        padding: 10px;
                    }
                }
            }
        }
    }
    
</style>