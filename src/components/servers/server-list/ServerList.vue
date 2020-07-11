<template>
    <div class="row">
        <div class="col-xs-12 col-sm-6">
            <ul class="list-group">
                <li
                        class="list-group-item"
                        v-for="index in 5">
                    <app-server-details :id="index"></app-server-details>
                </li>
            </ul>
        </div>
        <app-server-news></app-server-news>
    </div>
</template>

<script>
    import ServerNews from "../server-news/ServerNews.vue";
    import ServerDetails from "../server-details/ServerDetails.vue";

    export default {
        name: "ServerList",
        components:
            {
                'app-server-news': ServerNews,
                'app-server-details': ServerDetails
            }
    }
</script>

<style scoped>

</style>
