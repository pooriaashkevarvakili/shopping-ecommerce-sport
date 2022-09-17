<template>
    <div>
        <v-card height="250px" tile flat dark class="d-flex align-center justify-center mt-n10" color="#eff0f2">
            <v-row>
                <v-col cols="12" sm="12">
                    <h4 class="text-center mt-10 black--text">Subscribe to our news</h4>
                </v-col>
                <v-col cols="12" sm="12">
                    <h4 class="text-center mt-10 black--text">Lorem ipsum dolor sit amet consectetur adipisicing elit.
                        Fugiat magni at dicta consectetur eveniet vero recusandae deserunt nostrum neque, dolor, vel hic
                        commodi reiciendis doloribus, libero aspernatur numquam unde repudiandae?</h4>
                </v-col>
                <v-col cols="12" sm="12">
                    <v-card flat color="transparent" class="d-flex align-center justify-center">
                        <v-text-field dense filled append-icon="mdi-email-outline" background-color="grey" rounded
                            class="shrink" placeholder="enter your email">
                        </v-text-field>
                    </v-card>
                </v-col>
            </v-row>
        </v-card>
    </div>
</template>

<script>
export default {
    name: 'DashboardFiveView'
}
</script>

<style>
.card-2 {
    z-index: 1;
}
</style>