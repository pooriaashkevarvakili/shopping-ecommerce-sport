<template>

    <v-col cols="9" class="mt-n3">
        <v-row>
            <v-col cols="12" sm="4" v-for="(cloth,i) in clothes" :class="cloth.class" :key="i">
                <v-hover v-slot:default="{hover}">
                    <v-card height="300" align="center" flat outlined tile>
                        <v-card-actions>
                            <v-space></v-space>
                            <v-btn color="black" small dark>{{cloth.sold}}</v-btn>
                        </v-card-actions>
                        <v-img contain :src='cloth.image' width="200" height="200" />
                        <v-card-text class="mt-n4">
                            <strong :class="hover?'red--text':'black--text'">{{cloth.title}}</strong>
                        </v-card-text>
                        <v-expand-transition>
                            <div v-if="hover" style="height:100%"
                                class="d-flex v-card--reveal  display-3 white--text transition-fast-in-fast-out-blue">
                                <v-btn rounded color="white">
                                    <v-icon>mdi-cart-outline </v-icon>
                                    Buy
                                </v-btn>
                                <v-btn fab small color="white" class="ml-2">
                                    <v-icon color="black">mdi-content-copy</v-icon>
                                </v-btn>
                                <v-btn fab small color="white" class="ml-2">
                                    <v-icon color="black">mdi-heart-outline</v-icon>
                                </v-btn>
                            </div>
                        </v-expand-transition>
                    </v-card>
                </v-hover>
            </v-col>
        </v-row>

    </v-col>

</template>

<script>
export default {
    name: 'DashboardFourView',
    data: () => ({
        clothes: [
            {
                class: 'pa-0',
                sold: '-20%',
                image: 'shoeOne.jpg',
                title: 'shoeOne',
                price: '100',

            },
            {
                class: 'pa-0',
                sold: '-30%',
                image: 'shoeTwo.jpg',
                title: 'shoeTwo',
                price: '200',

            }, {
                class: 'pa-0',
                sold: '-40%',
                image: 'shoeThree.jpg',
                title: 'shoeThree',
                price: '300',

            }, {
                class: 'pa-0',
                sold: '-50%',
                image: 'shoeFour.jpg',
                title: 'shoeFour',
                price: '400',

            }, {
                class: 'pa-0',
                sold: '-60%',
                image: 'shoeFive.jpg',
                title: 'shoeFive',
                price: '500',

            }, {
                class: 'pa-0',
                sold: '-70%',
                image: 'shoeSix.jpg',
                title: 'shoeSix',
                price: '600',

            }, {
                class: 'pa-0',
                sold: '-80%',
                image: 'shoeSeven.jpg',
                title: 'shoeSeven',
                price: '700',

            }, {
                class: 'pa-0',
                sold: '-90%',
                image: 'shoeEight.jpg',
                title: 'shoeEight',
                price: '800',

            },

            {
                class: 'pa-0',
                sold: '-100%',
                image: 'shoeNine.jpg',
                title: 'shoeNine',
                price: '100',

            }
        ]
    })
}
</script>

<style>
.v-card--reveal {
    align-items: center;
    justify-content: center;
    bottom: 0;
    opacity: .5;
    position: absolute;
    width: 100%
}
</style>