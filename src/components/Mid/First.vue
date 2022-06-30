<template>
    <div id="main">
        <h1>Open new tabs is sh*t </h1>
        <div id="pini">
            <img id="mag" src="@/assets/left-mid.svg" alt="">
            <div id="imgg">
                <img src="@/assets/Group-15.svg" alt="" id="mag">
                <img src="@/assets/elon-mob.svg" id="mob">
            </div>
            <img src="@/assets/right-mid.svg" alt="" id="mag">
        </div>
        <p>A solution for your browser tabs and don’t make your device get slower over time. Get ease and faster to
            discover a trend with just one tab.</p>
    </div>
</template>

<script>
export default {
    name: "Fir-st"
}
</script>

<style scoped>
#main {
    background-color: #A8FF35;
    padding: 140px 292px;
}

#pini {
    display: flex;
}

h1 {
    width: 854px;
    height: 86px;
    margin-bottom: 60px;
    font-style: normal;
    font-weight: 700;
    font-size: 72px;
    line-height: 86px;
    text-align: center;
    color: #000000;
}

#imgg {
    width: 502px;
    height: 202px;
    margin: 0 auto 0 auto;
    background: #F5F5F5;
    border-radius: 16px;
    padding: 60px 80px;
}

p {
    width: 666px;
    height: 54px;
    margin-top: 60px;
    margin-left: 80px;
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 150%;
    text-align: center;
    color: #000000;
}

img {
    display: none;
}

#mag {
    display: block;
}

@media screen and (max-width: 375px) {
    #main {
        padding: 80px 14px;
    }

    h1 {
        width: 347px;
        height: 40px;
        font-style: normal;
        font-weight: 700;
        font-size: 34px;
        line-height: 112%;
        /* or 40px */

        text-align: center;

        color: #000000;
    }

    #imgg {
        width: 339px;
        height: 118px;
        background: #F5F5F5;
        border-radius: 14px;
        padding: 24px;
    }


    #mag {
        display: none;
    }

    #mob {
        display: block;
    }

    p {
        width: 286px;
        height: 63px;
        font-style: normal;
        font-weight: 400;
        font-size: 14px;
        line-height: 150%;
        text-align: center;
        color: #000000;
        margin: 34px auto 0 auto;
    }
}
</style>