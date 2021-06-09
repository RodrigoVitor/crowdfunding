<template>
    <div>
        <div class="container">
            <div class="barraDireita">
                <p>$89,914</p> 
                <small>of $100,000 backed</small>
            </div>

            <div class="barraDireita">
                <p>5,007</p>
                <small>total backers</small>
            </div>

            <div>
                <p>56</p>
                <small>days left</small>
            </div>
        </div>

        <div class="barra">
            <p>.</p>
        </div>
    </div>
</template>

<style scoped>
div {
    width:50%;
    margin: 40px auto auto auto;
    background:#fff;
    text-align: center;
    padding:0 0 5px 0;
    border-radius:10px
}
.container {
    display: grid;
    grid-template-columns: 250px 180px 150px;
}
.barraDireita {
    border-right:1px solid gray;
    padding-right:50px;
    border-radius: 0;
}
.container div {
    margin-left:-100px;
}
.container p {
    font-weight:bold;
    font-size:1.7rem
}
.container div > small {
    display: block;
    margin-top:10px;
    color:gray
}

.barra {
    background:gray;
    width:80%;
    margin-bottom:25px
}
.barra p {
    background:hsl(176, 72%, 28%);
    width:80%;
    border-radius:25px
}
@media screen and (max-width:980px) {
    .container {
        grid-template-columns:250px;
    }
    .container div {
        margin-left:0px;
    }
    .barraDireita {
        border-right:none
    }
}

</style>