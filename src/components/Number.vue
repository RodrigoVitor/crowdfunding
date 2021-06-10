<template>
    <div>
        <div id="number">
            <div class="container">
                <div class="barraVertical">
                    <p>$89,914</p>
                    <small>of $100,000 backed</small>
                </div>
                <div class="barraVertical">
                    <p>5,007</p>
                    <small>total hackers</small>
                </div>
                <div>
                    <p>56</p>
                    <small>days left</small>
                </div>
            </div>
            <div class="barra"><div></div></div>
        </div>
    </div>
</template>

<style scoped>
#number {
    width:50%;
    margin: 20px auto auto auto;
    background:#fff;
    text-align: center;
    padding:0 0 40px 0;
    border-radius:10px
}

/* Container */
.container {
    display:grid;
    grid-template-columns: 150px 150px 150px;
    padding-top:30px;
    justify-content: center;
}
.container div p {
    font-weight:bold;
    font-size:1.7rem;
}
.container div small {
    color:gray;
    display:block;
    margin-top:15px;
}
.barraVertical {
    border-right:1px solid gray
}
/* barra horizontal */
.barra {
    background:gray;
    width:80%;
    border-radius:25px;
    margin:35px auto auto auto;
   
}
.barra div {
    background:hsl(176, 72%, 28%);
    width:70%;
    height:10px;
    border-radius: 0 20px 20px 0
}

/* Landspace */
@media screen and (max-width:768px) {
    .container {
        grid-template-columns: 120px 120px 120px;
    }
    .container div p {
        font-size:1.5rem
    }
}
@media screen and (max-width:640px) {
    #number { width:70%}
}

/* Smartphones */
@media screen and (max-width:414px) {
    /* #number {
        width:70%;
    } */
    .container {
        grid-template-columns: auto;
    }
    .container div small {
        margin:5px 0 10px 0
    }
    .barraVertical {
        border:none
    }
}
</style>