<template>
    <div>
        <div id="mastercraft">
            <img src="../assets/logo-mastercraft.svg" alt="Logo-Mastercraft">
            <h1>Mastercraft Bamboo Monitor Riser </h1>
            <p>A beautiful and handcrafted monitor stand to reduce neck and eye strain</p>
            <div>
                <button>Back this project</button>
                <img src="../assets/icon-bookmark.svg" alt="bookmark">
                <button><img src="../assets/icon-bookmark.svg" alt="bookmark">Bookmark</button>
            </div>
        </div>
    </div>
</template>


<style scoped>
#mastercraft {
    width:50%;
    margin: -80px auto auto auto;
    background:#fff;
    text-align: center;
    padding:0 0 40px 0;
    border-radius:10px
}
#mastercraft > img {
    margin-top:-20px
}
#mastercraft p {
    color:hsl(0, 0%, 48%)
}
#mastercraft h1, p {
    margin-top:10px
}
#mastercraft > div {
    display:flex;
    justify-content: space-around;
    margin-top:30px;
}
#mastercraft div button > img {
    margin-right:20px
}
#mastercraft div > button:first-child {
    padding-left:30px;
    background-color:hsl(176, 72%, 28%);
    color:white;
}
#mastercraft div > img {visibility: hidden}

#mastercraft div > button {
    border-radius: 40px;
    display:flex;
    align-items: center;
    padding-right:30px;
    cursor:pointer;
    border:none;
}

@media screen and (max-width:720px) {
    #mastercraft {
        width: 70%;
        font-size: 14px;
    }
}

@media screen and (max-width:375px) {
    #mastercraft div > img {visibility: visible}
    #mastercraft div > button:last-child {display:none}
}

</style>

