<script>
export default {

    data() {
        return {
            pelatih: [
                { title: 'Pelatih', nama: 'Irsyaad Fatahilah', src: 'foo.png' },
                { title: 'Pelatih', nama: 'Fadhil Maulana', src: 'foo.png' },
                { title: 'Pelatih', nama: 'Iqbal Januar', src: 'BRB YELLOW.png' },
                { title: 'Pelatih', nama: 'Irsyaad Fatahilah', src: 'foo.png' },
                { title: 'Pelatih', nama: 'Fadhil Maulana', src: 'foo.png' },
                { title: 'Pelatih', nama: 'Iqbal Januar', src: 'BRB YELLOW.png' },
                // { title: 'Pelatih', src: 'BRB YELLOW.png' }
            ]
        }
    }

}
</script>
<template>
    <!-- Pelatih & Manajemen -->
    <v-main style="background-color: #181818;" class="pb-16">

        <v-container class="white--text" style="background-color: #181818;">

            <v-row>
                <v-col>
                    <h1>Pelatih dan <br> Manajemen</h1>
                    <p>berikut adalah Manajemen
                        dan pelatih dari <font color="#F7CC3E"> Bandung Run Bike </font>
                    </p>
                </v-col>
            </v-row>

            <v-row>
                <v-col v-for="(item, i) in pelatih" :key="i" class="justify-center d-flex">
                    <div>

                        <v-card outlined shaped class="my-5 py-10 card px-10 mx-6" color="#2D2D2D" min-width="240" max-width="245" max-height="245" min-height="300">
                            <v-img max-width="120px" max-height="120px" class="gambar_pelatih  mx-auto" :src="item.src"></v-img>
                            <!-- <v-card-title >Irsyaad Fatahilah</v-card-title> -->
                            <v-card-text>
                                <v-row justify="center" class="mx-0 mt-1">
                                    <font color="#F7CC3E" size="2" class="font-weight-light">{{ item.title }}</font>
                                </v-row>
                                <v-row justify="center" class="mx-0 mt-3">
                                    <font color="white" size="3">{{ item.nama }}</font>
                                </v-row>
                                <v-row justify="center" class="mx-0 mt-7">
                                    <v-img src="BRB YELLOW.png" max-width="20px"></v-img>
                                </v-row>
                            </v-card-text>
                        </v-card>
                    </div>
                </v-col>
            </v-row>

        </v-container>

    </v-main>
</template>


<style>
h1 {
    font-size: 45px;
    font-family: PoppinsSemiBold;
    margin-bottom: 10px;
}

p {
    font-family: PoppinsLight;
    font-size: 14px;
}

.gambar_pelatih {
    border-radius: 50% !important;
    border: 2px solid #F7CC3E !important;
}

.card {
    border: 2px solid #F7CC3E !important;
    transition-duration: 0.3s;

}

.card:hover {
    border: 2px solid #F7CC3E !important;
    box-shadow: 0px 0px 20px 0px rgba(255, 255, 255, 0.20), 0 0px 40px 0 rgba(255, 255, 255, 0.2);
}
</style>