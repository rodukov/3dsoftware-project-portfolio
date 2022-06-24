<template>
<div class="features">
    <div class="name-category">
        <p class="default main">Features</p>
        <p class="default desc">All features stored here</p>
    </div>
    <div class="features-grid">

        <div class="feature">
            <div class="imgc"><img src="../assets/icons8-folder-96.png" class="img"></div>
            <div class="text">
                <p class="default fmain">Archive storage</p>
                <p class="default fdesc">Lorem Ipsum is simply dummy text
                    of the printing and typesetting industry. Lorem Ipsum
                    has been the industry's standard dummy text ever
                    since the 1500s</p>
            </div>
        </div>

        <div class="feature">
            <div class="imgc"><img src="../assets/icons8-cloud-96.png" class="img"></div>
            <div class="text">
                <p class="default fmain">Cloud-based Platform</p>
                <p class="default fdesc">Lorem Ipsum is simply dummy text
                    of the printing and typesetting industry. Lorem Ipsum
                    has been the industry's standard dummy text ever
                    since the 1500s</p>
            </div>
        </div>

        <div class="feature">
            <div class="imgc"><img src="../assets/icons8-image-96.png" class="img"></div>
            <div class="text">
                <p class="default fmain">Export settings</p>
                <p class="default fdesc">Lorem Ipsum is simply dummy text
                    of the printing and typesetting industry. Lorem Ipsum
                    has been the industry's standard dummy text ever
                    since the 1500s</p>
            </div>
        </div>

        <div class="feature">
            <div class="imgc"><img src="../assets/icons8-code-64.png" class="img"></div>
            <div class="text">
                <p class="default fmain">Working with code</p>
                <p class="default fdesc">Lorem Ipsum is simply dummy text
                    of the printing and typesetting industry. Lorem Ipsum
                    has been the industry's standard dummy text ever
                    since the 1500s</p>
            </div>
        </div>

        <div class="feature">
            <div class="imgc"><img src="../assets/icons8-circle-96.png" class="img"></div>
            <div class="text">
                <p class="default fmain">Animations</p>
                <p class="default fdesc">Lorem Ipsum is simply dummy text
                    of the printing and typesetting industry. Lorem Ipsum
                    has been the industry's standard dummy text ever
                    since the 1500s</p>
            </div>
        </div>

        <div class="feature">
            <div class="imgc"><img src="../assets/icons8-gear-100.png" class="img"></div>
            <div class="text">
                <p class="default fmain">More render engines</p>
                <p class="default fdesc">Lorem Ipsum is simply dummy text
                    of the printing and typesetting industry. Lorem Ipsum
                    has been the industry's standard dummy text ever
                    since the 1500s</p>
            </div>
        </div>

        <div class="feature">
            <div class="imgc"><img src="../assets/icons8-interface-60.png" class="img"></div>
            <div class="text">
                <p class="default fmain">Nice Interface</p>
                <p class="default fdesc">Lorem Ipsum is simply dummy text
                    of the printing and typesetting industry. Lorem Ipsum
                    has been the industry's standard dummy text ever
                    since the 1500s</p>
            </div>
        </div>

        <div class="feature">
            <div class="imgc"><img src="../assets/icons8-open-source-100.png" class="img"></div>
            <div class="text">
                <p class="default fmain">Open Source</p>
                <p class="default fdesc">Lorem Ipsum is simply dummy text
                    of the printing and typesetting industry. Lorem Ipsum
                    has been the industry's standard dummy text ever
                    since the 1500s</p>
            </div>
        </div>

        <div class="feature">
            <div class="imgc"><img src="../assets/icons8-help-96.png" class="img"></div>
            <div class="text">
                <p class="default fmain">Сommunity</p>
                <p class="default fdesc">Lorem Ipsum is simply dummy text
                    of the printing and typesetting industry. Lorem Ipsum
                    has been the industry's standard dummy text ever
                    since the 1500s</p>
            </div>
        </div>

    </div>
</div>
</template>

<script>
export default { name: 'features' }
</script>

<style scoped>
.features {
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

.feature {
    background-color: #141414;
    border-radius: 25px;
    padding-left: 58px;
    padding-right: 58px;
    padding-top: 30px;
    padding-bottom: 30px;
    margin-top: 19px;
    transition: .11s;
}
.feature:hover {
    background-color: #1d1d1d9f;
}
.feature:hover > .imgc{
    background: #202020;
}

.fmain {
    font-family: 'Inter';
    font-style: normal;
    font-weight: 500;
    font-size: 25px;
    line-height: 30px;
    color: #CBCBCB;
    text-align: center;
    margin-top: 29px;

}
.fdesc {
    font-family: 'Inter';
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 24px;
    text-align: center;
    color: #888888;
    margin-top: 29px;
    margin-bottom: 46px;
}
.img {
    filter: invert(100%);
    width: 42px;
    height: 42px;
}
.imgc {
    background: #1A1A1A;
    border-radius: 35px;
    display: inline-block;
    padding-top: 37px;
    padding-bottom: 37px;
    padding-left: 44px;
    padding-right: 44px;
    
    display: table; margin: auto; /* Awesome center */
    

}
.features-grid {
    display: grid;
    grid-template-columns: 33.333333% 33.333333% 33.333333% ;
    column-gap: 17px;
}

@media (max-width: 1350px) {
    .features-grid { display: grid; grid-template-columns: 50% 50%; }
}
@media (max-width: 815px) {
    .features-grid { display: inline-block; }
}
@media (max-width: 869px) {
    .features { margin: 6px; }
}
</style>

