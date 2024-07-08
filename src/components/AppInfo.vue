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
    <section class="container">
        <div class="colonna">
            <ul>
                <li class="title">
                    <h3>{{  }}</h3>
                </li>
                <li>
                    <a href=""> {{ item }}</a>
                </li>
            </ul>
        </div>
        <div class="colonna">
            <ul>
                <li class="title">
                    <h3>{{  }}</h3>
                </li>
                <li>
                    <a href=""> {{ item }}</a>
                </li>
            </ul>
        </div>
        <div class="colonna">
            <ul>
                <li class="title">
                    <h3>{{  }}</h3>
                </li>
                <li>
                    <a href=""> {{ item }}</a>
                </li>
            </ul>
        </div>
        <div class="colonna">
            <ul>
                <li class="title">
                    <h3>{{  }}</h3>
                </li>
                <li>
                    <a href=""> {{ item }}</a>
                </li>
            </ul>
        </div>
        

    </section>

</template>

<style lang="scss" scoped>

@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap');

.container {
    background-image: url(/src/assets/dc-logo-bg.png), 
    url(/src/assets/footer-bg.jpg);
    background-repeat: no-repeat, repeat;
    background-position: right top, top left;
    padding: 3rem;
    .colonna {
        margin: 1.2rem 14rem;

        ul li {
            color: white;
            list-style: none;

            h3 {
                font-family: "Bebas Neue", sans-serif;
            }
            
            a {
                text-decoration: none;
                color: white;
            }
            
        }
    }
}

</style>