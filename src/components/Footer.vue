<template>
    <footer>
        <div class="pre-footer">
            <div class="container">
                <div class="col left">
                    <div class="inside-col">
                        <h3>DC COMICS</h3>
                        <ul>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Comics</a>
                            </li>
                            <li>
                                <a href="#">Movies</a>
                            </li>
                            <li>
                                <a href="#">TV</a>
                            </li>
                            <li>
                                <a href="#">Games</a>
                            </li>
                            <li>
                                <a href="#">Videos</a>
                            </li>
                            <li>
                                <a href="#">News</a>
                            </li>
                        </ul>
                        <h3>Shop</h3>
                        <ul>
                            <li>
                                <a href="#">Shop DC</a>
                            </li>
                            <li>
                                <a href="#">Shop DC Collectibles</a>
                            </li>
                        </ul>
                    </div>
                    <div class="inside-col">
                        <h3>DC</h3>
                        <ul>
                            <li>
                                <a href="#">Therms of use</a>
                            </li>
                            <li>
                                <a href="#">Privacy policy (new)</a>
                            </li>
                            <li>
                                <a href="#">Ad Choices</a>
                            </li>
                            <li>
                                <a href="#">Adversting</a>
                            </li>
                            <li>
                                <a href="#">Jobs</a>
                            </li>
                            <li>
                                <a href="#">Subscriptions</a>
                            </li>
                            <li>
                                <a href="#">Talent Workshops</a>
                            </li>
                            <li>
                                <a href="#">CPSC Certificates</a>
                            </li>
                            <li>
                                <a href="#">Ratings</a>
                            </li>
                            <li>
                                <a href="#">Shop Help</a>
                            </li>
                            <li>
                                <a href="#">Contact us</a>
                            </li>
                        </ul>
                    </div>
                    <div class="inside-col">
                        <h3>Sites</h3>
                        <ul>
                            <li>
                                <a href="#">DC</a>
                            </li>
                            <li>
                                <a href="#">Mad Magazine</a>
                            </li>
                            <li>
                                <a href="#">DC Kids</a>
                            </li>
                            <li>
                                <a href="#">DC Universe</a>
                            </li>
                            <li>
                                <a href="#">DC Power Visa</a>
                            </li>
                        </ul>
                    </div>
                    
                </div>
                <div class="col right">
                    <img id="footer-logo-bg" src="../assets/img/dc-logo-bg.png" alt="DC Footer Logo">
                </div>
            </div>
        </div>
        <div class="end-footer">
            <div class="container">
                <div class="col left">
                    <button>SIGN UP NOW!</button>
                </div>
                <div class="col right">
                    <h4>Follow us</h4>
                    <ul>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-facebook.png" alt="facebook">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-twitter.png" alt="twitter">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-youtube.png" alt="youtube">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-periscope.png" alt="periscope">
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

    footer{
        background-color: $brand-second-color;
        color: white;
        .pre-footer{
            background-image: url('../assets/img/footer-bg.jpg');
            background-repeat: no-repeat;
            background-size: cover;

            width: 100%;

            overflow: hidden;
            .container{
                display: flex;
                flex-flow: row nowrap;
                justify-content: flex-start;
                align-items: flex-start;
                .col.left{
                    height: 100%;
                    width: 50%;

                    padding: 30px 0;

                    display: flex;
                    flex-flow: row nowrap;
                    justify-content: flex-start;
                    align-items: flex-start;
                    .inside-col{
                        margin-right: 30px;
                    }
                    h3{
                        text-transform: uppercase;
                        margin: 20px 0;
                    }
                    ul{
                        list-style-type: none;
                        li{
                            font-weight: 100;
                            margin: 5px 0;
                            a{
                                text-decoration: none;
                                color: inherit;
                                font-weight: inherit;
                            }
                        }
                    }
                }
                .col.right{
                    #footer-logo-bg{
                        overflow: hidden;
                        margin: -70px 0px;
                    }
                }
            }
        }
        .end-footer{
            background-color: $brand-second-color;
            padding: 30px 0;
            .container{
                display: flex;
                flex-flow: row nowrap;
                justify-content: flex-start;
                align-items: center;
                .col{
                    button{
                        background-color: $brand-second-color;
                        color: white;
                        padding: 10px 15px;
                        text-align: center;
                        text-decoration: none;
                        display: inline-block;
                        font-size: 12px;
                        border: 1px solid $brand-main-color;
                        cursor: pointer;
                    }
                    h4{
                        color: $brand-main-color;
                        text-transform: uppercase;
                        margin: 0px 15px;
                    }
                    ul{
                        list-style-type: none;
                        li{
                            display: inline-block;
                            margin: 0px 5px;
                        }
                    }
                }
                .col.right{
                    margin-left: auto;
                    display: flex;
                    flex-flow: row nowrap;
                    justify-content: flex-start;
                    align-items: center;
                }
            }
        }
    }
</style>
