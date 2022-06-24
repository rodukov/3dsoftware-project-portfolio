<template>
<div class="download">
    <div class="name-category">
        <p class="default main">Download</p>
        <p class="default desc">You can download on all operating systems</p>
    </div>
    <div class="grid">
        <div class="download-item">
            <div class="download-items">
                <div class="imgc">
                    <img class="img" src="../assets/icons8-mac-client-96.png">
                </div>
                <p class="default text" style="margin-top: auto; margin-bottom: auto;">MacOS (M1)</p>
            </div>
        </div>

        <div class="download-item">
            <div class="download-items">
                <div class="imgc">
                    <img class="img" src="../assets/icons8-mac-client-96.png">
                </div>
                <p class="default text" style="margin-top: auto; margin-bottom: auto;">MacOS (Intel)</p>
            </div>
        </div>
        <div class="download-item">
            <div class="download-items">
                <div class="imgc">
                    <img class="img" src="../assets/icons8-windows8-96.png">
                </div>
                <p class="default text" style="margin-top: auto; margin-bottom: auto;">Windows 11</p>
            </div>
        </div>
        <div class="download-item">
            <div class="download-items">
                <div class="imgc">
                    <img class="img" src="../assets/icons8-windows8-96.png">
                </div>
                <p class="default text" style="margin-top: auto; margin-bottom: auto;">Windows 10</p>
            </div>
        </div>
        <div class="download-item">
            <div class="download-items">
                <div class="imgc">
                    <img class="img" src="../assets/ubuntu_icon_137064(3).png">
                </div>
                <p class="default text" style="margin-top: auto; margin-bottom: auto;">Ubuntu</p>
            </div>
        </div>
        <div class="download-item">
            <div class="download-items">
                <div class="imgc">
                    <img class="img" src="../assets/icons8-arch-linux-96.png">
                </div>
                <p class="default text" style="margin-top: auto; margin-bottom: auto;">Arch</p>
            </div>
        </div>
        <div class="download-item">
            <div class="download-items">
                <div class="imgc">
                    <img class="img" src="../assets/icons8-centos-96.png">
                </div>
                <p class="default text" style="margin-top: auto; margin-bottom: auto;">CentOS</p>
            </div>
        </div>
        <div class="download-item">
            <div class="download-items">
                <div class="imgc">
                    <img class="img" src="../assets/icons8-globe-96.png">
                </div>
                <p class="default text" style="margin-top: auto; margin-bottom: auto;">Web Version</p>
            </div>
        </div>

    </div>
</div>
</template>

<script>
export default { name: 'download' }
</script>

<style scoped>
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
.grid {
    display: grid;
    grid-template-columns: 24% 24% 24% 24%;
    column-gap: 20px;
}
.download {
    margin-left: 75px;
    margin-right: 75px;
    margin-top: 45px;
    margin-bottom: 45px;   
}
.download-item {
    padding-top: 150px;
    padding-bottom: 150px;
    padding-left: 40px;
    padding-right: 40px;
    background: #000000;
    border-radius: 25px;
    margin-bottom: 20px;
    transition: .2s;
}
.download-item:hover {
    background: radial-gradient(100% 100% at 100% 100%, #f475ff 0%, #80f6ff 34.9%, #ff8453 87.54%);
    transform: scale(1.01);
}

.download-items { display: flex; justify-content: center;}
.text {
    font-family: 'Inter';
    font-style: normal;
    font-weight: 500;
    font-size: 29px;
    line-height: 35px;
    text-align: center;
    color: #FFFFFF;
    margin-left: 25px;
}
.img {
    filter: invert(100%);
    height: 38px;
    width: 38px;

}

@media (max-width: 1537px ) {
    .grid { display: grid;
        grid-template-columns: 33% 33% 33%;
        column-gap: 20px; }
}

@media (max-width: 945px ) {
    .grid { display: grid;
        grid-template-columns: 50% 50%;
        column-gap: 20px; }
}

@media (max-width: 1537px ) {
    .grid {
        display: grid;
        grid-template-columns: 100%;
        column-gap: 20px;
     }
}
@media (max-width: 869px) {
    .download { margin: 6px ; }
}
</style>