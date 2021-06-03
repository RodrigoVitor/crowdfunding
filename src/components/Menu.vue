<template>
    <div>
        <nav>
            <img src="../assets/icon-hamburger.svg" alt="icon-hamburger" :class="[isClosed ? 'open-menu' : 'closed-menu']" @click="OpenClosedMenu">

            <img src="../assets/icon-close-menu.svg" alt="close-menu" :class="[isOpen ? 'open-menu' : 'closed-menu']" @click="OpenClosedMenu">
            
            <ul :class="[isOpen ? 'open-menu' : 'closed-menu']">
                <li><a href="#">About</a></li>
                 <li><a href="#">Discover</a></li>
                 <li><a href="#">Get started</a></li>
            </ul>
        </nav>
    </div>
</template>

<script>
export default {
    data: function() {
        return {
            isOpen: false,
            isClosed: true
        }
    },
    methods: {
        OpenClosedMenu() {
            this.isOpen = !this.isOpen
            this.isClosed = !this.isClosed
        }
    }
}
</script>

<style scoped>
/* reset */
ul {list-style: none;}
a{text-decoration: none; color: rgba(255, 255, 255, 0.822)}
/* ----------- */

/* Menu */
div {
    position: absolute; 
    right:40px;
    top:75px;}
nav img {
    cursor: pointer;
}
/* Menu */
.closed-menu {visibility: hidden;}
.open-menu {visibility: visible;}

/* Largura minima */
@media screen and (min-width: 720px) {
    nav {display:none}
}
/* Tablet */
@media screen and (max-width: 720px) {
    nav ul {
        background:white;
        width:500px;
        position:absolute;
        top:90px;
        right:15px;
        border-radius:20px
    }
    nav ul li {
        border-bottom: 1px solid gray;
        padding:30px 0 30px 20px
    }
    nav ul li a {
        color:black;
        font-size: 1.3rem;
    }
}
/* smartphones */
@media screen and (max-width:540px) {
    nav ul{
        width:350px;
    }
}

@media screen and (max-width:375px) {
    nav ul{
        width:250px;
    }
}

@media screen and (max-width:320px) {
    nav ul{
        right:5px
    }
}

</style>