<template>
<div class="welcome">
    <div class="welcome-text">
        <p class="default main">New<br> <span class="main-gradient">generation</span><br> of 3D<br> Software</p>
        <p class="default desc">Use matter. Use sculpting.<br> Modern engines. Feel like a fish in water in 3D.</p>
    </div>
    <div class="vector-draw">
        <img src="../assets/Vector.png" class="imgv">
    </div>
    
</div>
</template>

<script>
export default {
    name: 'welcome'
}
</script>

<style scoped>
.welcome { 
    margin-left: 75px;
    margin-right: 75px;
    display: flex;
    margin-top: 45px;
    margin-bottom: 45px;
}
.main {
    font-family: 'Inter';
    font-weight: 800;
    font-size: 100px;
    color: #FFFFFF;
}
.desc {
    font-family: 'Inter';
    font-weight: 800;
    font-size: 32px;
    color: #d8d8d8;  
    margin-top: 44px;
}
.main-gradient {
    background: linear-gradient(95.57deg, #9C79FF 3.13%, #59D6BF 90.2%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}
@keyframes main-gradient-animation {
    0% {
        background: rgb(0, 238, 255);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
    }
    50% {
        background: rgb(119, 0, 255);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
    }
    100% {
        background: rgb(0, 238, 255);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
    } 
}

.vector-draw {
    margin-left: auto;
    margin-right: auto;
}

@media (max-width: 1413px) {

    .vector-draw { position: absolute; z-index: -1; }
}
@media (max-width: 869px) {
    .imgv {
        height: 80%;
        width: 80%;
    }
    .main { font-size: 70px; }
    .desc { font-size: 22px; }
    .welcome { margin: 6px ; }
}
</style>