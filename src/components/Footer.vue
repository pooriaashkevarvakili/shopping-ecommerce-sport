

<template>
    <v-footer dark padless>
        <v-card flat title class="white--text black py-12 px-5" width="100%">
            <v-row>
                <v-col cols="12" sm="4">
                    <v-card-text class="white--text pt-0">
                        <h3>AAEIDELPRO</h3>
                    </v-card-text>
                    <v-card-text class="grey--text pt-0">
                        <h3>
                            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Vel, doloremque sunt! Velit
                            accusamus aliquid inventore vero laudantium corrupti, illo amet, perferendis expedita totam
                            maiores accusantium rem blanditiis doloribus praesentium saepe!
                        </h3>
                    </v-card-text>
                    <v-toolbar flat color="transparent">
                        <h5 class="ml-4">Gudies</h5>
                        <h5 class="ml4">Terms of use</h5>
                        <h5 class="ml4">Privacy policy</h5>
                    </v-toolbar>
                    <v-card-text>&#169;20212022</v-card-text>
                </v-col>
                <v-col cols="12" sm="2">
                    <v-card-text class="white--text pt-0">
                        <h3>Get Help</h3>
                    </v-card-text>
                    <v-card-text class="grey--text pt-0">
                        <h3>orderstatus</h3>
                    </v-card-text>
                    <v-card-text class="grey--text mt-n4">
                        <h3>
                            shoppinganddelivery
                        </h3>
                    </v-card-text>
                    <v-card-text class="grey--text mt-n4">
                        <h3>
                            paymentOptions
                        </h3>
                    </v-card-text>
                    <v-card-text class="grey--text mt-n4">
                        <h3>
                            contact us
                        </h3>
                    </v-card-text>
                </v-col>
                <v-col cols="12" sm="2">
                    <v-card-text class="white--text pt-0">
                        <h3>Aboutus</h3>
                    </v-card-text>
                    <v-card-text class="grey--text pt-0">
                        <h3>Carees</h3>
                    </v-card-text>
                    <v-card-text class="grey--text mt-n4">
                        <h3>
                            sustainability
                        </h3>
                    </v-card-text>
                    <v-card-text class="grey--text mt-n4">
                        <h3>
                            Service
                        </h3>
                    </v-card-text>
                    <v-card-text class="grey--text mt-n4">
                        <h3>
                            CA Supply Chains Act
                        </h3>
                    </v-card-text>
                </v-col>
                <v-col cols="12" sm="4">
                    <v-card-text class="pt-0">
                        <v-btn v-for="icon in icons" icon class="mx-1 white--text" :key="icon">
                            <v-icon size="24px">
                                {{icon}}
                            </v-icon>
                        </v-btn>
                    </v-card-text>
                    <v-card-text class="grey--text mt-14">
                        payment methods:
                    </v-card-text>
                    <v-toolbar flat color="transparent">
                        <v-spacer></v-spacer>
                        <v-icon large>fab fa-cc-visa</v-icon>
                        <v-icon large>fab fa-cc-paypal</v-icon>
                    </v-toolbar>
                </v-col>
            </v-row>
        </v-card>
    </v-footer>
</template>

<script>
export default {
    name: "FooterView",
    data: () => ({
        icons: [
            'mdi-facebook',
            'mdi-twitter',
            'mdi-linkedin',
            'mdi-instagram'
        ]



    }),
}
</script>

<style>

</style>