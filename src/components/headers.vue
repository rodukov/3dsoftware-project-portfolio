<template>
<div class="headers">
        <div class="logo"></div>
    <div class="header-items-left">

        <div class="header-item-container"><p class="header-item default">Updates</p></div>
        <div class="header-item-container"><p class="header-item default">Source</p></div>
        <div class="header-item-container"><p class="header-item default">Twitter</p></div>
        <div class="header-item-container"><p class="header-item default">Community</p></div>
    </div>
    <div class="header-items-right">
        <div class="header-download-container" style="display: inline-block; margin-top: auto; margin-bottom: auto; margin-right: auto; "><p class="header-download default">Download</p></div>
    </div>
</div>
</template>

<script>
export default { name: 'headers' }
</script>

<style scoped>
.headers {
    display: flex; 
    background: red;
    margin-left: auto;
    margin-right: auto;
    max-width: 828px;
    max-height: 117px;
    background: rgba(9, 9, 9, 0.49);
    border-radius: 35px;
    padding: 20px;
    padding-left: 30px;
    padding-right: 30px;
    margin-top: 18px; margin-bottom: 18px;
    backdrop-filter: blur(15px);

}
.header-items-left { 
    display: flex;
    align-items: left;
    justify-content: left;
}
.logo {
    width: 77px;
    height: 77px;
    background: radial-gradient(90.91% 84.93% at 0% 17.53%, #41E251 0%, #00E0FF 50.38%, #DB00FF 100%) /* warning: gradient uses a rotation that is not supported by CSS and may not behave as expected */;
    border-radius: 30px;

}
.header-items-right {
    display: flex;
    align-items: right;
    justify-content: right;
    text-align: right;
    margin-left: auto;
}
.header-item-container {
    display: inline-block;
    margin-top: auto; 
    margin-bottom: auto;
    padding: 25px; 
}
.header-item {
    color: white;
    font-family: 'Inter';
    font-weight: 700;
    font-size: 20px;
    position: relative;
    animation: vlasik .3s;
}

/* Underline animation */
.header-item:after {
  content: '';
  position: absolute;
  width: 100%;
  transform: scaleX(0);
  height: 2px;
  bottom: -13px;
  left: 0;
  background: linear-gradient(45deg, rgb(227, 113, 255), rgb(70, 128, 255), rgb(71, 219, 212), rgb(181, 255, 97) );
  padding: 1px;
  border-radius: 5px;
  transform-origin: bottom right;
  transition: transform 0.12s ease-out;
}
.header-item:hover:after { transform: scaleX(1); transform-origin: bottom left; }


.header-item:hover { cursor: pointer; }
.header-download {
    /* Button */
    position: relative;
    box-sizing: border-box;
    padding: 14px;
    padding-left: 58px;
    padding-right: 58px;
    font-family: 'Inter';
    font-style: normal;
    font-weight: 700;
    font-size: 20px;
    color: #FFFFFF;

    
    transition: .1s;
}
.header-download:hover {
    cursor: pointer;
    filter: drop-shadow(0px 4px 0px #00C2FF);
}
.header-download:before {
  content: "";
  position: absolute;
  inset: 0;
  border-radius: 35px; 
  padding: 2px; 
  background:linear-gradient(90deg, #E048D1, #5CD8FF, #FF7051); 
  -webkit-mask: 
     linear-gradient(#fff 0 0) content-box, 
     linear-gradient(#fff 0 0);
  -webkit-mask-composite: xor;
          mask-composite: exclude; 
}
</style>