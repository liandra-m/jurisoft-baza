<script setup>
    import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
    import {library} from '@fortawesome/fontawesome-svg-core';
    import {faAngleDown, faAngleUp, faBars} from '@fortawesome/free-solid-svg-icons';
    import Menu from './menu/menu.vue';

    library.add(faAngleDown);
    library.add(faAngleUp);
    library.add(faBars);
</script>

<script>
    export default {
        data() {
            return {
                section: {
                    0: false,
                    1: false,
                    2: false,
                    3: false,
                },
                sectionTimeOut: null,
            }
        },
        methods: {
            showSection (index){
                clearInterval(this.sectionTimeOut);

                for (let i of Object.keys(this.section)) {
                    if (i != index)
                        this.section[i] = false;
                }

                return this.section[index] = true;
            }, 

            hideSection (index) {
                this.sectionTimeOut = setTimeout(() => {
                    this.section[index] = false;
                }, 500);
                
            },

            handleSection (index) {
                return this.section[index] = !this.section[index];
            }
        }
    }
</script>

<template>
    <div class="nav">
        <h1 class="brand">
            Baza
        </h1>
        <div class="desktop">
            <div class="nav-items">
                <a href="#shop">
                    Shop
                </a>
                <a href="#sell" :class="section[0] ? 'active' : null" @mouseenter="showSection(0)" @mouseleave="hideSection(0)">
                    Sell Online
                    <font-awesome-icon v-if="section[0]" :icon="['fa','angle-up']" />
                    <font-awesome-icon v-else :icon="['fa','angle-down']" />
                    <Menu v-if="section[0]" :items="['My account', 'Cart', 'Checkout']" :positionX="80"></Menu>
                </a>
                <a href="#blog" :class="section[1] ? 'active' : null" @mouseenter="showSection(1)" @mouseleave="hideSection(1)">
                    Blog
                    <font-awesome-icon v-if="section[1]" :icon="['fa','angle-up']" />
                    <font-awesome-icon v-else :icon="['fa','angle-down']" />
                    <Menu v-if="section[1]" :items="['Blog one column', 'Blog one column with sidebar', 'Blog two columns', 'Blog two columns with sidebar']" :positionX="160"></Menu>
                </a>
                <a href="#contact" :class="section[2] ? 'active' : null" @mouseenter="showSection(2)" @mouseleave="hideSection(2)">
                    Contact Us
                    <font-awesome-icon v-if="section[2]" :icon="['fa','angle-up']" />
                    <font-awesome-icon v-else :icon="['fa','angle-down']" />
                    <Menu v-if="section[2]" :items="['Contact us 1', 'Contact us 2', 'Contact us 3', 'Contact us 4']" :positionX="300"></Menu>
                </a>
                <button class="btn btn-grey">
                    Buy now
                </button>
                
            </div>
        </div>

        <div class="mobile">
            <div class="nav-items">
                <font-awesome-icon class="hamburguer" :icon="['fa','bars']" />
            </div>
        </div>

    </div>
</template>

<style scoped>
    @import './navbar.css';
</style>