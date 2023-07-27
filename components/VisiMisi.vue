<template>
    <v-main style="background-color: #181818;">
        
        <v-container fluid style="background-image: url('vimi_bg.png') ; background-size: cover;  height: 130vh">
            <v-container>
                <v-row class="d-flex justify-center">
                    <v-btn dropzone="" fab x-large color="#F7CC3E" style=" margin-top: 27px;">
                        <v-img src="BRB BLACK.png" max-width="35px"></v-img>
                    </v-btn>
                </v-row>

                <v-container class="pt-16">

                    <v-row class="d-flex justify-center pt-2">
                        <h2>Visi & Misi BRB</h2>
                    </v-row>

                    <v-row class="mt-16 pt-10 text-left d-flex ">
                        <v-col cols="6">
                            <h2>Visi</h2>
                            <p>memiliki pengertian suatu gagasan yang tertuang dalam bentuk tulisann tentang tujuan khusus
                                atau
                                utama dari suatu organisasi atau instansi</p>
                        </v-col>
                    </v-row>

                    <v-row class="mt-10 text-right d-flex justify-end">
                        <v-col cols="6">
                            <h2>Misi</h2>
                            <p>memiliki pengertian suatu gagasan yang tertuang dalam bentuk tulisann tentang tujuan khusus
                                atau
                                utama dari suatu organisasi atau instansi asdasd asd memiliki pengertian suatu gagasan yang
                            </p>

                            <v-btn outlined small class="text-capitalize py-4 px-5 style_btn text-caption " to="/program">
                                Program
                            </v-btn>
                        </v-col>
                    </v-row>
                </v-container>
            </v-container>
        </v-container>
    </v-main>
</template>

<style>
.style_btn {
    transition-duration: 3s;
}

.style_btn:hover {
    background-color: #F7CC3E;
    transition-duration: 0.3s;
}</style>