<script>
    export default {
        props: ['items', 'positionX'],
    }
</script>

<template>
    <div class="menu-box" :style="{left: this.positionX + 'px'}">
        <ul>
            <li v-for="item in items">
                <a :href="'#' + item.replace(/ /g, '-').toLowerCase()">{{ item }}</a>
            </li>
        </ul>
    </div>
</template>

<style scoped>
    @import './menu.css';
</style>