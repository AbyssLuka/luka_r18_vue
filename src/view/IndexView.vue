<template>
    <div class="index">
        <div class="router-view-container">
            <router-view></router-view>
        </div>
        <header-menu class="header-menu"></header-menu>
    </div>
<!--        <cursor-osu></cursor-osu>-->
</template>

<script setup lang="ts">
    // import FloatingWindow from "@/components/module/FloatingWindow";
    import HeaderMenu from "@/components/module/HeaderMenu.vue";
    // import CursorOsu from "@/components/module/Cursor.vue";
</script>

<style scoped>

    .header-menu {
        min-height: 75px;
        height: auto;
        width: 100vw;
        backdrop-filter: blur(10px);
        background: rgba(255, 255, 255, 0.5);
    }

    .router-view-container {
        width: 100%;
        height: calc(100% - 75px);
    }

    .index {
        display: flex;
        flex-direction: column-reverse;
        width: 100vw;
        height: 100vh;
        background-size: cover;
    }


</style>