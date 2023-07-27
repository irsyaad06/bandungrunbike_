<script>
export default {
    name: 'NavBar',

    data() {
        return {
            navbar: [
                { title: 'Tentang BRB', to: '/' },
                { title: 'Program', to: '/program' },
                { title: 'Galeri', to: '/galeri' }
            ]
        }
    }
}
</script>

<template>
    <v-main style="background-color: #181818;">
        <v-app-bar app hide-on-scroll elevate-on-scroll color="#181818">
            <v-container>
                <v-container class="d-flex align-center">
                    <router-link class="router-link white--text" to="/"><v-img src="BRB YELLOW.png"
                            max-width="45px"></v-img></router-link>
                    <v-spacer></v-spacer>
                    <router-link v-for="(item, i) in navbar" :key="i" :to="item.to" class="router-link ml-6 "> {{ item.title
                    }} </router-link>

                    <!-- manual title of navbar-->
                    <!-- <router-link class="router-link white--text" to="/">Tentang BRB</router-link>
                    <router-link class="router-link mx-5 white--text" to="/program">Program</router-link>
                    <router-link class="router-link white--text" to="/galeri">Galeri</router-link> -->

                </v-container>
            </v-container>
        </v-app-bar>
    </v-main>
</template>

<style>
h6 {}

.router-link {
    font-size: 14px;
    font-family: PoppinsLight;
    text-decoration: none;
    color: azure !important;
}

.router-link:hover {
    color: #F7CC3E !important;
}

.nuxt-link-exact-active {
    color: #F7CC3E !important;
}
</style>

