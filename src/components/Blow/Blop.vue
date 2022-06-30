<template>
    <div id="bash">
        <h1>All platform connect to Findtrend</h1>
        <div id="poco">
            <div v-for="pic in pico" :key="pic.id" class="paca" :id="pic.id">
                <img :src="pic.url" alt="">
            </div>
        </div>
        <div id="und">
            <div v-for="tweet in twee" :key="tweet.id" :id="tweet.id">

                <img :src="tweet.url" alt="">
            </div>
        </div>
        <div id="mond">
            <div v-for="mono in mondo" :key="mono.id" :id="mono.id">

                <img :src="mono.url" alt="">
            </div>
        </div>
        <but3 ButtonText="View More Trend" id="but3"></but3>
    </div>
</template>

<script>
import but3 from "@/components/Button.vue"
export default {
    name: "Blo-p",
    components: { but3 },
    data() {
        return {
            pico: [
                { id: "hap1", url: require("@/assets/Facebook.svg") },
                { id: "hap2", url: require("@/assets/Twitter.svg") },
                { id: "hap3", url: require("@/assets/Ball.svg") },
                { id: "hap4", url: require("@/assets/pinterest.svg") },
                { id: "hap5", url: require("@/assets/Mako.svg") },
                { id: "hap6", url: require("@/assets/reddit.svg") },
                { id: "hap7", url: require("@/assets/Wakawaka.svg") },
                { id: "hap8", url: require("@/assets/LinkedIn.svg") }
            ],
            twee: [
                { id: "tw1", url: require("@/assets/tweet1.svg") },
                { id: "tw2", url: require("@/assets/tweet2.svg") },
                { id: "tw3", url: require("@/assets/tweet3.svg") }
            ],
            mondo: [
                { id: "mon1", url: require("@/assets/tweet1-mob.svg") },
                { id: "mon2", url: require("@/assets/tweet2-mob.svg") },
                { id: "mon3", url: require("@/assets/tweet3-mob.svg") }
            ]
        }
    }
}
</script>

<style scoped>
#hap2 {
    background: #A8FF35
}

#bash {
    padding: 140px;
    background: #FAFAFA;
}

#poco {
    display: flex;
    gap: 24px;
    margin-top: 80px;
    overflow: auto;
}

h1 {
    height: 76px;
    left: 140px;
    top: 3378px;
    font-style: normal;
    font-weight: 700;
    font-size: 64px;
    line-height: 76px;
    text-align: center;
    color: #000000;
}

#und {
    margin-top: 76px;
    gap: 32px;
    display: flex;
    flex-direction: column;

}

#und img {
    display: block;
    margin-left: auto;
    margin-right: auto;
}

.paca {
    width: 110px;
    height: 110px;
    background: #FFFFFF;
    border-radius: 8px;
    padding: 24px;
}

#mond {
    display: none;
}

@media screen and (max-width: 375px) {
    h1 {
        width: 339px;
        height: 86px;
        font-style: normal;
        font-weight: 900;
        font-size: 36px;
        line-height: 43px;
        text-align: center;
        color: #000000;
    }

    #bash {
        padding: 80px 18px;
    }

    #poco img {
        width: 30px;
    }

    .paca {
        width: 64px;
        height: 64px;
        padding: 16px;
    }

    #und {
        display: none;
    }

    #mond {
        display: block;

    }

    #mond img {
        display: block;

        margin-left: auto;
        margin-right: auto;
    }

    #mon1 {
        padding: 32px 0 16px 0;
    }

    #mon3 {
        padding: 16px 0 32px 0;
    }

    #but3 {
        margin-top: 0;
    }
}
</style>