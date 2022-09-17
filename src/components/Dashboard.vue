
<template>
    <v-container>
        <v-card color="#3853d8" height="150px" class="d-flex align-center justify-center " dark>
            <v-row>
                <v-col cols="12" sm="12">
                    <h4 class="text-center">MensLifeStyleShoes</h4>
                </v-col>
                <v-col cols="12" sm="12">
                    <v-breadcrumbs dark :items="items" class="justify-center mt-n7">
                        <template v-slot:divider>
                            <v-icon color="#7c92fe">mdi-chevron-right</v-icon>
                        </template>
                    </v-breadcrumbs>
                </v-col>
            </v-row>

        </v-card>
        <v-card tile class="mx-16 mt-n10 card1" color="white">
            <v-row>
                <v-col cols="12" sm='8' class="pr-0">
                    <v-card height="250px" tile flat color="#3893d8">
                        <v-row>
                            <v-col cols="12" sm="4" class="pl-8 pt-5">
                                <v-btn small tile color="black" dark class="withoutuppercase">New</v-btn>
                                <h6 class="white--text mt-8">MOUNTINE BIKE</h6>
                                <h3 class="white--text mt-5">Trek Speed Concept</h3>
                                <v-btn dark rounded class="withoutuppercase px-8 mt-10" color="#4c9cdb">MoreInfo</v-btn>
                            </v-col>

                        </v-row>
                    </v-card>
                </v-col>
                <v-col class="pl-0" cols="12" sm="4">
                    <v-card height="250px" tile flat color="#6857e1">
                        <v-row>
                            <v-col cols="12" sm="6" class="pl-8 pt-5">
                                <v-btn dark color="black" class="withoutuppercase">New</v-btn>
                                <h6 class="white--text mt-8">Down jocket</h6>
                                <h3 class="white--text mt-5">Sale Collection</h3>
                                <v-btn rounded color="#8353e7" class="px-8 mt-3" dark>
                                    MoreInfo
                                </v-btn>
                            </v-col>

                        </v-row>
                    </v-card>
                </v-col>
            </v-row>
            <v-row>
                <v-col cols="12" class="mt-n6 pr-0" sm="3">
                    <v-toolbar flat outlined>
                        <v-toolbar-title>
                            <strong>Filter</strong>
                        </v-toolbar-title>
                        <v-spacer></v-spacer>
                        <v-divider vertical></v-divider>
                        <v-btn icon class="ml-1">
                            <v-icon color='#3853d8'>
                                mdi-sync
                            </v-icon>
                        </v-btn>
                    </v-toolbar>
                </v-col>
                <v-col cols="12" sm="3" class="mt-n6 px-0">
                    <v-toolbar flat outlined>
                        <v-toolbar-title>
                            SPORTBY:<span>PRICE</span>
                        </v-toolbar-title>
                        <v-spacer></v-spacer>
                        <v-btn icon class="mr-4">
                            <v-icon>mdi-menu-down</v-icon>
                        </v-btn>
                    </v-toolbar>
                </v-col>
                <v-col cols="12" sm="3" class="mt-n6 px-0">
                    <v-toolbar flat outlined>
                        <v-toolbar-title>
                            SHOW:<span>12</span>
                        </v-toolbar-title>
                        <v-spacer></v-spacer>
                        <v-btn icon class="mr-4">
                            <v-icon color="black">mdi-menu-down</v-icon>
                        </v-btn>
                    </v-toolbar>
                </v-col>
                <v-col cols="12" sm="3" class="mt-n6 pl-0">
                    <v-toolbar flat>
                        <v-btn icon>
                            <v-icon color="#3853d8 ">mdi-apps</v-icon>
                        </v-btn>
                        <v-divider vertical></v-divider>
                        <v-btn class="mx-1" icon>
                            <v-icon color="grey">mdi-format-list-bulleted</v-icon>
                        </v-btn>
                        <v-divider vertical></v-divider>
                        <v-toolbar-title>
                            <strong>Compage:</strong>
                        </v-toolbar-title>
                        <v-spacer></v-spacer>
                        <v-badge color="#3853d8" content="3" class="mr-2 " />
                    </v-toolbar>
                </v-col>
                <v-col cols="3" md="12" lg="3" sm='12' xs="12" xl='12' class="responsive-one py-0 pr-0 mt-n3">
                    <v-card flat outlined tile>
                        <v-toolbar flat>
                            <v-icon color="black" class="mr-2">mdi-chevron-down</v-icon>
                            <strong>CATEGORIE</strong>
                            <v-spacer></v-spacer>
                            <v-icon color="grey">mdi-close</v-icon>
                        </v-toolbar>
                        <v-list dense class="mt-n5">
                            <v-list-item v-for="style in styles" :key="style.ttile">
                                <v-list-item-content>
                                    <v-list-item-title class="ml-8" v-text="style.ttile"></v-list-item-title>
                                </v-list-item-content>
                                <v-list-item-action>
                                    <v-list-item-subtitle v-text="style.count"></v-list-item-subtitle>
                                </v-list-item-action>
                            </v-list-item>
                        </v-list>
                    </v-card>
                    <v-card flat outlined>
                        <v-toolbar flat>
                            <v-icon color="black" class="mr-2">mdi-chevron-down</v-icon>
                            <strong>PRICE</strong>
                            <v-spacer></v-spacer>
                            <v-icon color="grey">mdi-close</v-icon>
                        </v-toolbar>
                        <v-toolbar flat>
                            <v-text-field rounded filled dense class="mx-2" placeholder="$50"></v-text-field>

                            <v-text-field rounded filled dense class="mx-2" placeholder="$1900"></v-text-field>
                        </v-toolbar>
                        <v-range-slider color="blue" max="40" min="-30"></v-range-slider>
                    </v-card>
                    <v-card flat outlined tile>
                        <v-toolbar flat>
                            <v-icon color="black" class="mr-2">mdi-chevron-down</v-icon>
                            <strong>BRAND</strong>
                            <v-spacer></v-spacer>
                            <v-icon color="grey" small>mdi-close</v-icon>
                        </v-toolbar>
                        <v-list class="mt-n5">
                            <v-list-item v-for="brand in brands" :key="brand.title">
                                <v-list-item-content>
                                    <v-list-item-title class="ml-6" v-text="brand.title"></v-list-item-title>
                                </v-list-item-content>
                                <v-list-item-action>
                                    <v-checkbox color="primary" v-model="brand.state" />
                                </v-list-item-action>
                            </v-list-item>
                        </v-list>
                    </v-card>
                    <v-card flat outlined tile>
                        <v-toolbar flat>
                            <v-icon color="black" class="mr-2">mdi-chevron-down</v-icon>
                            <strong>Color</strong>
                            <v-spacer></v-spacer>
                            <v-icon color="grey" small>mdi-close</v-icon>
                        </v-toolbar>
                        <v-chip-group column multiple>
                            <v-chip :outlined="item.outlined" :class="item.class" :filter="item.filter"
                                v-for="item in chips" :key="item.color" :text-color="item.textColor"
                                :color="item.color">
                            </v-chip>
                        </v-chip-group>
                    </v-card>
                    <v-card>
                        <v-toolbar flat>
                            <v-icon color="black" class="mr-2">mdi-chevron-down</v-icon>
                            <strong>Size</strong>
                            <v-spacer></v-spacer>
                            <v-icon color="grey" small>mdi-close</v-icon>
                        </v-toolbar>
                        <v-chip-group column multiple active-class="blue white--text">
                            <v-chip v-for="(item,index) in sizes" :key="index" :value="sizes" :class="sizes">
                                {{item}}
                            </v-chip>

                        </v-chip-group>
                    </v-card>
                </v-col>
                <DashboardFour />
                <v-col cols="12" sm='3' class="mt-n3 pr-0 pb-0">
                    <v-toolbar flat outlined></v-toolbar>

                </v-col>
                <v-col cols="12" sm='3' class="mt-n3 px-0 pb-0">
                    <v-toolbar flat outlined></v-toolbar>
                    <v-btn icon class="mr-1">
                        <v-icon color="grey">mdi-chevron-up</v-icon>
                    </v-btn>
                    <v-divider vertical></v-divider>
                </v-col>
                <v-col cols="12" sm="3" class="mt-n3 px-0 pb-0">
                    <v-toolbar flat outlined class="text-center">
                        <v-pagination class="responsive-two" style="margin-left:-20px" v-model="page" :length="4">
                        </v-pagination>
                    </v-toolbar>
                </v-col>
                <v-col cols="12" sm='3' class="mt-n3 pl-0 pb-0">
                    <v-toolbar flat outlined>
                        <v-btn icon class="mr-1">
                            <v-icon color="grey">mdi-chevron-down </v-icon>
                        </v-btn>
                        <v-divider vertical></v-divider>
                    </v-toolbar>

                </v-col>
            </v-row>
        </v-card>
        <DashboardFive />
    </v-container>
</template>

<script>

import DashboardFour from "./DashboardFour.vue";
import DashboardFive from "./DashboardFive.vue"
export default {
    name: 'DashboardView',
    components: { DashboardFour, DashboardFive },
    data: () => ({
        page: 1,
        sizes: [
            '35', '36', '37', '38', '39', '40', '41', '42', '43', '44', '45', '46',
        ],

        chips: [
            {
                class: "ml-2",
                filter: true,
                outlined: true,
                color: "black",
                textColor: "black"
            },
            {
                color: "black",
                filter: true,
                textColor: 'white'
            },
            {
                color: '#e6e6e6',
                filter: true,
                textColor: 'white'
            },
            {
                color: '#ffb500',
                filter: true,
                textColor: 'white'
            },
            {
                color: '#27229',
                filter: true,
                textColor: 'white'
            },
            {
                color: '#eb3427',
                filter: true,
                textColor: 'white'
            },
            {
                color: '#9223fa3',
                filter: true,
                textColor: 'white'
            },
            {
                class: 'ml-2',
                filter: true,
                color: '#3a51df',
                textColor: 'white'

            },
            {

                filter: true,
                color: '#23a7f5',
                textColor: 'white'

            },
            {
                filter: true,
                color: '#5eb524',
                textColor: 'white'

            },
            {
                filter: true,
                color: '#7c5f4d',
                textColor: 'white'

            },
            {
                filter: true,
                color: 'black',
                textColor: 'white'

            },
            {
                filter: true,
                color: 'lime',
                textColor: 'white'

            },
        ],
        brands: [
            {
                title: 'lifestyle',
                state: true
            },
            {
                title: 'Running',
                state: false
            },
            {
                title: 'trading & Gym',
                state: true
            },
            {
                title: 'basketball',
                state: false
            }
        ],
        items: [
            {
                text: 'Home',
                disabled: false,
                href: 'breadcrumbs-home'
            },
            {
                text: 'Catalog',
                disabled: false,
                href: 'breadcrumbs-catalog'
            },
            {
                text: 'Men',
                disabled: false,
                href: 'breadcrumbs-men'
            }, {
                text: 'Shoes',
                disabled: false,
                href: 'breadcrumbs-shoes'
            }
        ],
        styles: [
            {
                ttile: "lifestyle",
                count: 1
            },
            {
                ttile: "runinig",
                count: 2
            },
            {
                ttile: "trading",
                count: 45
            },
            {
                ttile: "basketball",
                count: 11
            },
            {
                ttile: "Football",
                count: 15
            },
            {
                ttile: "soccer",
                count: 32
            },
            {
                ttile: "basketball",
                count: 8
            },
            {
                ttile: "golf",
                count: 15
            },
            {
                ttile: "shakebording",
                count: 22
            },
        ],
    }),
}
</script>

<style>
.container {
    padding: 0 !important;
}

.v-btn.withoutuppercase {
    text-decoration: none;
}

.v-chip.v-size__default {
    border-radius: 50px !important;
    font-size: 14px !important;
    height: 40px !important;
    width: 40px !important;
}

.v-card--reveal {
    align-items: center;
    justify-content: center;
    bottom: 0;
    opacity: .5;
    position: absolute;
    width: 100%
}

.card-1 {
    z-index: 10;
}

.card-2 {
    z-index: 1;
}

@media only screen and (max-width:594px) {
    .responsive-one {
        display: none
    }


}

@media screen and (max-width:1246px) {
    .responsive-two {
        display: none;
    }
}
</style>