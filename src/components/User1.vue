<template>
    <div class="card">
        <div class="card-body text-center" style="font-weight: bold" >
            <p> {{ baslik }}</p>
            <p> {{ deger }}</p>


        </div>
    </div>
</template>

<script>
    export default {
        name: "User1",
        props: {
            baslik: {
                type: String,
                require: true
            },

            deger: {
                type: String,
                require: true

            },
        },

    }
</script>

<style scoped>


</style>