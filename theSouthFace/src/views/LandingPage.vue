<template>
        <div class="content">
            <h1>THE SOUTH FACE</h1>
            <br>
            <h4>For a better typing experience.</h4><br>

            <div>
                <RouterLink to="/"><button type="button">proceed<span></span></button></RouterLink>
            </div>
        </div>
</template>

<style>

.content{
    width: 100%;
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    text-align: center;    
    color: white;
}
.content h1{
    font-size: 90px;
    margin-top: 40px;
}

.content a{
    color: white;
    text-decoration: none;
}
button{
    width: 200px;
    padding: 15px 0;
    text-align: center;
    text-transform: uppercase;
    text-size-adjust: 30px;
    margin: 20px 10px;
    border-radius: 20px;
    color: rgb(255, 255, 255); 
    font-weight: bold;
    border: 2px solid white;
    background: transparent;
    cursor: pointer;
    position: relative;
    overflow: hidden;
}
span{
    background: linear-gradient(rgba(202, 165, 0, 0.555), rgba(202, 165, 0, 0.555) );
    height: 100%;
    width: 0;
    border-radius: 20px;
    position: absolute;
    left: 0;
    bottom: 0;
    z-index: -1;
    transition: 0.5s;
}
button:hover span{
    width: 100%;
}

button:hover{
    color: white;
}
</style>
