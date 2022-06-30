<template>
    <div id="mim">
        <h1>Minimize your tabs.</h1>
        <h1>Find the trends!</h1>
        <div id="mup">
            <p>Don’t let your computer memories consumes all of those browser tabs.

                Findtrend let you gathers all of your favorite website into one place.</p>
        </div>
        <div id="bit">
            <but2 ButtonText="Get Started 🔥" id="but2"></but2>
            <img src="@/assets/img-hero.svg" alt="">
        </div>

    </div>
    <div id="ink">
        <img src="@/assets/btn-hero-socmed.svg" alt="">
    </div>
</template>

<script>
import but2 from "@/components/Button.vue"
export default {
    name: "Mid-head",
    components: { but2 },
    data() {
        return {

        }
    }
}
</script>

<style scoped>
h1 {
    height: 81px;
    font-style: normal;
    font-weight: 900;
    font-size: 72px;
    line-height: 112%;
    text-align: center;
    color: #FFFFFF;
    margin-left: auto;
    margin-right: auto;
}

#mim {
    margin-top: 100px;
    margin-bottom: 94px;
}

#mup {
    margin-top: 24px;
    margin-bottom: 40px;
}

p {
    width: 600px;
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 120%;
    text-align: center;
    color: #8B8B8B;
    /* display: block; */
    margin-left: auto;
    margin-right: auto;
}

img {
    display: block;
    margin: 0 auto 0 auto;
    padding-bottom: 92px;
}

#bit img {
    padding: 0;
    margin: 0;
}

#bit {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 18px;
}

@media screen and (max-width: 375px) {
    h1 {
        width: 350px;
        height: 40px;
        font-style: normal;
        font-weight: 900;
        font-size: 36px;
        line-height: 112%;
        text-align: center;
        color: #FFFFFF;
    }

    p {
        width: 286px;
        height: 84px;
        left: 45px;
        top: 240px;

        font-family: 'Effra';
        font-style: normal;
        font-weight: 400;
        font-size: 14px;
        line-height: 150%;
        /* or 21px */

        text-align: center;

        color: #8B8B8B;
    }

    #mim {
        margin-top: 56px;
        margin-bottom: 94px;
    }

    #ink {
        display: none;
    }

    #mup {
        margin-top: 16px;
        margin-bottom: 32px;
    }

    #bit img {
        display: none;
    }
}
</style>