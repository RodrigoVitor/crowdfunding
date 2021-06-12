<template>
    <div>
        <div class="container">
            <h1>About this project</h1>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ad sit necessitatibus saepe ullam dignissimos omnis nesciunt iste debitis culpa quisquam. Omnis fuga labore dicta recusandae tempora laudantium iste! Quae, reprehenderit.</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus, officiis assumenda, dolorum, nihil obcaecati officia laborum saepe itaque nostrum exercitationem incidunt adipisci possimus magnam id suscipit minus. Eum, in sed.</p>

            <div class="component-bamboo">
                <h2>Bamboo Stand  <small>Pledge $25 or more</small></h2>
                <p>You get an ergonomic stand made of natural bamboo. You've helped us launch our promotional campaign, and you'll be added t a special backer member list.</p>
                <div class="main">
                    <h1>101 <small>left</small></h1>
                    <button>Select Reward</button>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.container {
    width:50%;
    margin: 20px auto auto auto;
    background:#fff;
    text-align: center;
    padding:25px 0 40px 0;
    border-radius:10px
}
.container > h1 {
    font-size:1.4rem;
    text-align:left;
    margin-left:50px
}
.container > p {
    text-align: justify;
    margin:20px  50px;
    color:gray;
    line-height: 30px;
}
/* component-bamboo */
.component-bamboo {
    border:1px solid #ccc;
    width:80%;
    margin: auto;
    padding:20px;
    border-radius:10px
}
.component-bamboo > h2 {
    font-size:1.2rem;
    display:flex;
    justify-content: space-between;
}
.component-bamboo h2 > small {
    font-size:0.7rem;
    color:hsl(176, 72%, 28%)
}
.component-bamboo > p {
    text-align: justify;
    font-size:1rem;
    margin-top:20px;
    color:gray;
    line-height:30px
}
.component-bamboo h1 {
    display:flex;
    align-items: center;
    margin-top:25px
}
.component-bamboo h1 > small {
    font-size:.8rem;
    color:gray
}
.main {
    display:flex;
    justify-content: space-between;
    align-items: center;
}
.component-bamboo button {
    width:150px;
    height:50px;
    background-color: hsl(176, 50%, 47%);
    color:white;
    border:none;
    border-radius:25px;
    cursor:pointer;
}
/* Smartphones */
@media screen and (max-width:640px) {
    .container { width:70%}
    .container > p {
        line-height: 20px;
        text-align:left
    }
    /* component-bamboo */
    .component-bamboo {
        width:60%;
    }
    .component-bamboo > h2 {
        display:flex;
        flex-direction: column;
    }
    .component-bamboo > p {
        text-align: left;
        line-height:20px
    }
    .main {
        display:flex;
        flex-direction: column;
    }
}
</style>