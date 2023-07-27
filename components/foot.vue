<template>
    <v-footer padless>
        <v-card flat tile class="white--text text-center" width="100%" color="#F7CC3E">
            <v-card-text class="tea white--text text-center">
                <v-btn v-for="icon in icons" :key="icon" class="mx-4 white--text" icon>
                    <v-icon size="24px">
                        {{ icon }}
                    </v-icon>
                </v-btn>
               Footer
            </v-card-text>
         

            <v-divider></v-divider>

            <v-card-text class="white--text" >
                All rights Reserved. © {{ new Date().getFullYear() }} — <strong>now</strong> Bandung Run Bike
            </v-card-text>
        </v-card>
    </v-footer>
</template>

<script>
export default {
    name: 'FooterBar',
    data: () => ({
        icons: [
            'mdi-youtube',
            'mdi-instagram',
        ],
    }),
}
</script>

<style>
.tea{
    background-color: #181818;
}
</style>