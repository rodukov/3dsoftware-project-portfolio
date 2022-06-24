<template>
<div class="contact">
    <div class="text">
        <p class="default main">Contact</p>
        <p class="default desc">If you have suggestions, please use the contacts below.</p>
    </div>
    <div class="grid">
        <div class="socialc"><p class="socialn">📧 E-mail</p></div>
        <div class="socialc"><p class="socialn">🤖 Discord</p></div>
        <div class="socialc"><p class="socialn">🐦 Twitter</p></div>
        <div class="socialc"><p class="socialn">✉️ Telegram</p></div>
        <div class="socialc"><p class="socialn">💻 Github</p></div>
        <div class="socialc"><p class="socialn">📕 YouTube</p></div>
        <div class="socialc"><p class="socialn">📺 Tiktok</p></div>
        <div class="socialc"><p class="socialn">📷 Instagram</p></div>
        <div class="socialc"><p class="socialn">🙂 Facebook</p></div>
        <div class="socialc"><p class="socialn">📌 Pinterest</p></div>
    </div>
</div>
</template>

<script>
export default {
    name: 'contact'
}
</script>

<style scoped>
.contact {
    margin-left: 75px;
    margin-right: 75px;
    margin-top: 45px;
    margin-bottom: 45px;   
}
.main {
    font-family: 'Inter';
    font-style: normal;
    font-weight: 700;
    font-size: 50px;
    line-height: 61px;
    text-align: center;
    color: #E1E1E1;  
}
.desc {
    font-family: 'Inter';
    font-style: normal;
    font-weight: 700;
    font-size: 25px;
    line-height: 30px;
    text-align: center;
    color: #CBCBCB;
    margin-top: 19px;
    margin-bottom: 19px;
}
.socialc {
    padding-top: 66px;
    padding-bottom: 66px;
    padding-left: 41px;
    padding-right: 41px;
    box-sizing: border-box;
    border: 1px solid #343434;
    border-radius: 25px;
    transition: 0.1s;
}
.socialc:hover {
    background: rgba(51, 51, 51, 0.596);
}
.socialc:hover > .socialn{
    animation: bounce 0.8s;

}
@keyframes bounce {
   0%, 20%, 50%, 80%, 100% {transform: translateY(0);} 
   40% {transform: translateY(-30px);} 
   60% {transform: translateY(-15px);} 
} 
.socialn {
    transition: 0.1s;
    font-family: 'Inter';
    font-style: normal;
    font-weight: 400;
    font-size: 25px;
    line-height: 30px;
    text-align: center;

    color: #FFFFFF;
}
.grid {
    display: grid;
    grid-template-columns: 19% 19% 19% 19% 19%;
    gap: 22px;
}

@media (max-width: 1385px) {
    .grid
    {
    display: grid;
    grid-template-columns: 24% 24% 24% 24%;        
    }
}
@media (max-width: 1107px) {
    .grid
    {
    display: grid;
    grid-template-columns: 32% 32% 32%;        
    }
}
@media (max-width: 881px) {
    .grid
    {
    display: grid;
    grid-template-columns: 49% 49%;        
    }
}
@media (max-width: 609px) {
    .grid
    {
    display: grid;
    grid-template-columns: 100%;        
    }
}
@media (max-width: 869px) {
    .contact { margin: 6px ; }
}
</style>