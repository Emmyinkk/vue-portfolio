<template>
   <div class="navbar">
        <div class="container" id="header">
            <div class="navbar_header">
                <a class="logo" href="#">OO</a>
                    <button @click="onClick" class="hamburger" id="open">
                        <div class="menu"></div>
                        <div class="menu"></div>
                        <div class="menu"></div>
                    </button>
            </div>
    
            <nav id="nav2">
                <button @click="onClick2"><i class="fas fa-times exit" id="exit"></i></button>
                <ul class="list">
                    <li class="list_items active-link"><a href="#hero">About me</a></li>
                    <li class="list_items"><a href="#skills">My Skills</a></li>
                    <li class="list_items"><a href="#portfolio">Portfolio</a></li>
                    <li class="list_items"><a href="#contact">Get in touch</a></li>
                </ul>
            </nav>
        </div>
    </div>
</template>

<script>
import style from './style.css'
export default {
    name: 'Navbar',
    components: {
        style
    },
    created() {
        window.addEventListener('scroll', this.onScroll);
    },
    destroyed() {
        window.removeEventListener('scroll', this.onScroll);
    },
    methods: {
        onClick() {
            const navMenu = document.getElementById('nav2')
            
            if(navMenu.classList.contains('show-menu') === false) {
                navMenu.classList.add('show-menu');
            }
        },
        onClick2() {
            const navMenu = document.getElementById('nav2')
            
            if(navMenu.classList.contains('show-menu') === false) {
                navMenu.classList.add('show-menu');
            } else {
                navMenu.classList.remove('show-menu');
            }
        },
        onScroll() {
            const header = document.getElementById('header')
            if(window.scrollY >= 100) {
                header.classList.add('scroll-header')
            } else {
                header.classList.remove('scroll-header')
            }
        },
    }
}
</script>

<style scoped>
 button {
     background: transparent;
     border: none;
 }
</style>