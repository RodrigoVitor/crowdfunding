<template>
    <div>
        <nav>
            <img src="../assets/icon-hamburger.svg" alt="icon-hamburger">
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
div {
    position: absolute; 
    right:40px;
    top:40px;}
nav img {
    cursor: pointer;
}
@media screen and (min-width: 720px) {
    nav {display:none}
}
@media screen and (max-width: 720px) {
    nav ul {display:none}
}

</style>