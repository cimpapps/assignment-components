<template>
    <div class="container">
        <app-header title="Server Status"></app-header>
        <hr>
        <app-server-list></app-server-list>
        <hr>
        <app-footer></app-footer>

    </div>
</template>

<script>
    import AppHeader from "./components/header/AppHeader.vue";
    import AppFooter from "./components/footer/AppFooter.vue";
    import ServerList from "./components/servers/server-list/ServerList.vue";

    export default {
        components: {
            'app-header': AppHeader,
            'app-footer': AppFooter,
            'app-server-list': ServerList
        }
    }

</script>

<style>

</style>
