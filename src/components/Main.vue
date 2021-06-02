<template>
    <div>
        <nav>
            <h2>crowdfunding</h2>
            <div>
                <ul>
                    <li><a href="#">About</a></li>
                    <li><a href="#">Discover</a></li>
                    <li><a href="#">Get started</a></li>
                </ul>
            </div>
            <Menu />
        </nav>
    </div>
</template>

<script>
import Menu from '../components/Menu'
export default {
    components: {
        Menu
    }
}
</script>

<style scoped>
/* reset */
ul {list-style: none;}
a{text-decoration: none; color: rgba(255, 255, 255, 0.822)}
/* -------------------- */
nav {
    display:flex;
    justify-content: space-between;
    background-image:url('../assets/image-hero-desktop.jpg');
    height:400px
}
nav h2, ul {
    color:white;
    margin-top:40px
}
nav h2 {margin-left:175px}
nav ul{margin-right:85px}
nav ul li {
    display:inline-block;
    margin-left:15px
}

@media screen and (max-width: 720px) {
    nav {
        background-image:url('../assets/image-hero-mobile.jpg');
        height:600px
    }
    nav ul {
        display:none
    }
    nav h2 {margin-left:55px;font-size: 2rem;}
}
@media screen and (max-width: 375px) {
    nav {display:none}
}
</style>