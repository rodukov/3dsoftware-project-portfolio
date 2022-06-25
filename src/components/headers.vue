<template>
<div class="adaptive-headers">
    <button class="menu" v-on:click="add_active()" onclick="this.classList.toggle('opened');this.setAttribute('aria-expanded', this.classList.contains('opened'))" aria-label="Main Menu">
      <svg width="100" height="100" viewBox="0 0 100 100">
        <path class="line line1" d="M 20,29.000046 H 80.000231 C 80.000231,29.000046 94.498839,28.817352 94.532987,66.711331 94.543142,77.980673 90.966081,81.670246 85.259173,81.668997 79.552261,81.667751 75.000211,74.999942 75.000211,74.999942 L 25.000021,25.000058" />
        <path class="line line2" d="M 20,50 H 80" />
        <path class="line line3" d="M 20,70.999954 H 80.000231 C 80.000231,70.999954 94.498839,71.182648 94.532987,33.288669 94.543142,22.019327 90.966081,18.329754 85.259173,18.331003 79.552261,18.332249 75.000211,25.000058 75.000211,25.000058 L 25.000021,74.999942" />
      </svg>
    </button>
    
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
</div>
</template>

<script>
export default {
    name: 'headers',
    data() { return { active: false }},
    methods: {
        add_active: function() {
            this.active = !this.active
            var element = document.querySelector(".headers");
            if(this.active) { element.classList.add("active"); }
            else { element.classList.remove("active"); }
        }
    }
}
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


.menu {
  background-color: transparent;
  border: none;
  cursor: pointer;
  display: flex;
  padding: 0;
  display: none;
}
.line {
  fill: none;
  stroke: rgb(255, 255, 255);
  stroke-width: 6;
  transition: stroke-dasharray 600ms cubic-bezier(0.4, 0, 0.2, 1),
    stroke-dashoffset 600ms cubic-bezier(0.4, 0, 0.2, 1);
}
.line1 {
  stroke-dasharray: 60 207;
  stroke-width: 6;
}
.line2 {
  stroke-dasharray: 60 60;
  stroke-width: 6;
}
.line3 {
  stroke-dasharray: 60 207;
  stroke-width: 6;
}
.opened .line1 {
  stroke-dasharray: 90 207;
  stroke-dashoffset: -134;
  stroke-width: 6;
}
.opened .line2 {
  stroke-dasharray: 1 60;
  stroke-dashoffset: -30;
  stroke-width: 6;
}
.opened .line3 {
  stroke-dasharray: 90 207;
  stroke-dashoffset: -134;
  stroke-width: 6;
}

@media (max-width: 914px) {
    .adaptive-headers {
        width: 100%;
        height: 100%;
        margin-bottom: 35px;
    }
    .headers {
        display: inline-block;
        width: 100%;
        background: inherit;
        margin: 0; padding: 0;
        transform: translateX(-100%);
        transition: 0.4s;
        position: absolute;
    }


    .active {
        transform: translateX(0%);
    }
    
    .adaptive-headers {
        background: rgb(0, 0, 0);
    }
    .headers {
        background: rgb(0, 0, 0);
        border-radius: 0;
    }
    .header-items-left {
        background: rgb(0, 0, 0);
    }
    .header-items-right {
        background: rgb(0, 0, 0);
        border-radius: 0px 0px 25px 25px;
    }
    .header-items-right {
        padding-bottom: 56px;
    }


    .logo { margin: auto; }
    .header-items-left {
        margin: auto;
        display: block;

    }
    .header-item-container {
        width: 100%;
        padding: 0;
        padding-bottom: 20px;
        padding-top: 20px;
    }
    .header-item {
        text-align: center;
    }
    .header-download-container {
        padding: 0;
        margin: auto;
    }


    .menu {
        display: block;
    }
}

</style>