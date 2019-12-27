<template>
    <div>
        <h1>Board List</h1>
        
        <v-btn icon text>
            <v-icon>mdi-plus</v-icon>
            Create new Project
        </v-btn>

        <v-divider></v-divider>
            
        <v-spacer></v-spacer>
        <Board
            v-for="project in projects"
            :key="project.name"
            v-bind:project_name=project.name>
        </Board>
        
    </div>
</template>

<script>
import Board from "../components/board";

export default {
    components: { Board },
    data: () => ({
        projects: [
            {
                id: 1,
                name: 'create trello cron'
            },
            {
                id: 2,
                name: 'make job description'
            },
        ]
    })
}
</script>