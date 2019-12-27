<template>
    <v-card
        class="mx-auto"
        max-width="344"
        outlined>
            <v-list-item
                three-line>
                <v-list-item-content>
                    <v-list-item-title>{{project_name}}</v-list-item-title>
                    <v-divider></v-divider>
                    <v-list-item-subtitle>created by Koji.oura</v-list-item-subtitle>
                    <v-list-item-subtitle>lastupdate: 2019/12/22 00:00:00</v-list-item-subtitle>
                </v-list-item-content>
            </v-list-item>

            <v-card-actions>
                <v-btn text>Show details</v-btn>
            </v-card-actions>
        </v-card>
</template>
<script>
export default {
    name: "board",
    props: ['project_name'],
    data: () => ({})
}
</script>