<template>
    <main>
        <h1>Homepage</h1>
        <div>
            <h2>This is the home page</h2>
            <div>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quos, quaerat. Exercitationem dolorem quo aliquam ratione quia. Harum doloribus atque assumenda. Quos aspernatur laudantium quibusdam. Placeat expedita excepturi quis id quidem?
                </p>
                <p>
                    <v-btn color="primary">
                        Button
                    </v-btn>
                </p>
            </div>
        </div>
        <div>
            <DataTableServer />
        </div>
    </main>
</template>

<script setup lang="ts">

</script>

<style scoped>
    h1{
        color: red;
    }
    h2{
        color:blue;
    }
    p{
        font-weight: bold;
        font-size: 1rem;
    }
</style>