
<template>
    <v-app-bar app color="#3853d8" dark>
        <v-btn icon>
            <v-icon>
                mdi-magnify
            </v-icon>
        </v-btn>
        <v-divider vertical class="ml-1 mr-3"></v-divider>
        <v-btn icon>
            <v-icon>mdi-menu</v-icon>
        </v-btn>
        <v-toolbar-title>
            <span class="caption">select</span><br>category
        </v-toolbar-title>
        <v-divider vertical></v-divider>
        <div class="text-center mx-auto Idlepro">
            <h4>AAe IdlePro</h4>
        </div>
        <v-spacer></v-spacer>
        <v-divider vertical />
        <v-btn icon>
            <v-icon>mdi-account-outline</v-icon>
        </v-btn>
        <v-divider vertical></v-divider>
        <v-btn icon class="mx-1">
            <v-badge content='2' color="#94d0ef">
                <v-icon>
                    mdi-cart-outline
                </v-icon>
            </v-badge>
        </v-btn>
    </v-app-bar>
</template>

<script>
export default {
    name: 'NavbarView'
}
</script>

<style>
.Idlepro {
    position: absolute;
    left: 0;
    right: 0;
}

.v-toolbar__title {
    font-size: 1rem !important;
}

.v-badge__badge {
    font-size: 10px !important;
    height: 18px !important;
    min-width: 18px !important;
}
</style>