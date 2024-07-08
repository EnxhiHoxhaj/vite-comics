<script>
export default {
    name: 'AppInfo',
    data () {
        return {
            linksFooter:[
                {
                    title: 'DC COMICS',
                    menuItems: [
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV', 
                        'Games',
                        'Videos',
                        'News',
                    ]
                },
                {
                    title: 'SHOP',
                    menuItems: [
                        'Shop DC',
                        'Shop DC Collectiones',
                    ]
                },
                {
                    title: 'DC',
                    menuItems: [
                        'Terms Of Use',
                        'Privacy policy (New)',
                        'Ad Choices',
                        'Adverstising', 
                        'Jobs',
                        'Subscriptions',
                        'Talent Workshops',
                        'CPSC Certifications',
                        'Ratings',
                        'shop Help',
                        'Conctact Us', 
                    ]
                },
                {
                    title: 'DC COMICS',
                    menuItems: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe', 
                        'DC Power Visa',
                    ]
                },
            ]
        }
    }
}

</script>

<template>
    <section class="container">
        <div class="colonna" v-for="( info, index) in linksFooter" key="index">
            <ul>
                <li class="title">
                    <h3>{{ info.title }}</h3>
                </li>
                <li>
                    <a href=""> {{ info.menuItems }}</a>
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

        }
    }
}

</style>