<template>
    <div>
        <nav>
            <img src="../assets/icon-hamburger.svg" alt="icon-hamburger" id="open-menu">
            <img src="../assets/icon-close-menu.svg" alt="close-menu" id="close-menu">
            <ul>
                <li><a href="#">About</a></li>
                 <li><a href="#">Discover</a></li>
                 <li><a href="#">Get started</a></li>
            </ul>
        </nav>
    </div>
</template>

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
#close-menu {visibility: hidden;}

/* Largura minima */
@media screen and (min-width: 720px) {
    nav {display:none}
}
/* Tablet */
@media screen and (max-width: 720px) {
    nav ul {display:none}
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