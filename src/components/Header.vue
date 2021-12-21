<template>
    <header>
        <div class="container">
            <nav>

                <img src="../assets/img/dc-logo.png" alt="DC Logo">

                <ul>
                    <li v-for="(link, index) in links" :key="index">
                        <a :href="link.url">{{ link.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
  name: 'Header',
  data: function() {
      return {
          links: [
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
                text: 'Tv',
                url: '#',
              },
              {
                text: 'Games',
                url: '#',
              },
              {
                text: 'Collectibles',
                url: '#',
              },
              {
                text: 'Videos',
                url: '#',
              },
              {
                text: 'Fans',
                url: '#',
              },
              {
                text: 'News',
                url: '#',
              },
              {
                text: 'Shop',
                url: '#',
              },
          ]
      }
  }
};
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

    header{
        background-color: white;
        nav{
            display: flex;
            flex-flow: row nowrap;
            justify-content: flex-start;
            align-items: center;

            color: $brand-second-color;
            font-size: 12px;
            text-transform: uppercase;
            font-weight: 600;
            height: 103px;
            img{
                height: 90%;
            }
            ul{
                margin-left: auto;
                list-style-type: none;
                li{
                    display: inline-block;
                    margin: auto 10px;
                    line-height: 100px;
                    border-bottom: 3px solid transparent;
                    cursor: pointer;
                    &:hover{
                        border-bottom: 3px solid $brand-main-color;
                        color: $brand-main-color;
                    }
                    a{
                        text-decoration: none;
                        color: inherit;
                        text-transform: inherit;
                        line-height: inherit;
                    }
                }
            }
        }
        
    }
</style>
