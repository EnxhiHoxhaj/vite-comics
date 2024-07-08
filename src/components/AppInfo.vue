<script>
export default {
    name: 'AppInfo',
    data () {
        return {
            comics:[
                {
                    text: 'DC COMICS',
                    url: '#'
                },
                {
                    text: 'Characters',
                    url: '#'
                },
                {
                    text: 'Comics',
                    url: '#'
                },
                {
                    text: 'Movies',
                    url: '#'
                },
                {
                    text: 'TV',
                    url: '#'
                },
                {
                    text: 'Games',
                    url: '#'
                },
                {
                    text: 'Videos',
                    url: '#'
                },
                {
                    text: 'News',
                    url: '#'
                },
            ],
            shop: [
            {
                    text: 'SHOP',
                    url: '#'
                },
                {
                    text: 'Shop DC',
                    url: '#'
                },
                {
                    text: 'Shop DC Collectiones',
                    url: '#'
                },
            ],
            dc:[
                {
                    text: 'DC',
                    url: '#'
                },
                {
                    text: 'Terms Of Use',
                    url: '#'
                },
                {
                    text: 'Privacy policy (New)',
                    url: '#'
                },
                {
                    text: 'Ad Choices',
                    url: '#'
                },
                {
                    text: 'Adverstising',
                    url: '#'
                },
                {
                    text: 'Jobs',
                    url: '#'
                },
                {
                    text: 'Subscriptions',
                    url: '#'
                },
                {
                    text: 'Talent Workshops',
                    url: '#'
                },
                {
                    text: 'CPSC Certifications',
                    url: '#'
                },
                {
                    text: 'Ratings',
                    url: '#'
                },
                {
                    text: 'Shop Help',
                    url: '#'
                },
                {
                    text: 'Conctact Us',
                    url: '#'
                },
            ],
            dcComics:[
                {
                    text: 'DC COMICS',
                    url: '#'
                },
                {
                    text: 'DC',
                    url: '#'
                },
                {
                    text: 'MAD Magazine',
                    url: '#'
                },
                {
                    text: 'DC Kids',
                    url: '#'
                },
                {
                    text: 'DC Universe',
                    url: '#'
                },
                {
                    text: 'DC Power Visa',
                    url: '#'
                },

            ]

        }
    }
}

</script>

<template>
    <section >
        <div class="container">
            <div class="colonna">
            <div class="dc_comics">
                <ul v-for="(itemComics, index0) in comics" key="index0">
                    <li>
                        <a href="#"> {{ itemComics.text }} </a>
                    </li>
                </ul>
            </div>
            <div>
                <ul v-for="(itemShop, index1) in shop" key="index1">
                    <li>
                        <a href="#"> {{ itemShop.text }} </a>
                    </li>

                </ul>
            </div>
        </div>
        <div class="colonna">
            <div>
                <ul v-for="(itemDc, index1) in dc" key="index1" >
                    <li>
                        <a href="#"> {{ itemDc.text }} </a>
                    </li>

                </ul>
            </div>
        </div>
        <div class="colonna">
            <div>
                <ul v-for="(itemDcComics, index1) in dcComics" key="index1">
                    <li>
                        <a href="#"> {{ itemDcComics.text }} </a>
                    </li>
                </ul>
            </div>
        </div>
        </div>
        
    </section>

</template>

<style lang="scss" scoped>

@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap');
section {
    background-image: url(src/assets/footer-bg.jpg);
    background-size: cover;
    position: relative;
}
.container {
    background-position-x: calc(100vw - 45rem) ;
    background-image: url(src/assets/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-size: 30%;
    padding: 3rem 0;
    font-size: 0.9rem;
    display: flex;

    .colonna {
        width: calc(40% / 3);

        &:first-child {
            margin-left:14rem;

            .dc_comics {
                margin-bottom: 1.2rem;
            }
        }

        ul {

            &:first-child {
                margin-bottom: 0.4rem;
                font-size: 1.5rem;
                font-family: "Bebas Neue", sans-serif;
                color: white;

                a {
                    color: white;
                }
            }

            li {
                color: white;
                list-style: none;    
                a {
                    text-decoration: none;
                    color:$light_text;
                }           
            }
        }
    }
}

</style>