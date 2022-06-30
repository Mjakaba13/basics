<template>
    <div id="uni">
        <h1>Get your best deal</h1>
        <div id="vash">
            <p id="mont">Monthly</p>
            <img src="@/assets/toggle.svg" alt="">
            <p id="yea">Yearly</p>
            <img src="@/assets/word.svg" alt="">
        </div>
        <div id="cards">
            <div v-for="tot in totem" :key="tot.id" :id="tot.min" class="pop">
                <p id="popo">{{ tot.txt }}</p>
                <p id="momo">{{ tot.tet }}</p>
                <hr>
                <div id="ion">
                    <h2>{{ tot.amt }}</h2>
                    <p id="hun">/Month</p>
                </div>
                <ul v-for="tit in tot.inne" :key="tit.ids">
                    <li> {{ tit.info }}</li>
                </ul>
                <but4 ButtonText="Start Free Trial" :id="tot.id">
                </but4>
            </div>
        </div>
    </div>
</template>

<script>
import but4 from "@/components/Button.vue"
export default {
    name: "Best-Deal",
    components: { but4 },
    data() {
        return {
            totem: [
                {
                    id: "see1", min: "sep1", txt: "Personal", tet: "Special first packet for all", amt: "$8", inne: [
                        { ids: "in1", info: "Up to 5 page each group" },
                        { ids: "in2", info: "Up to 10 group page" },
                        { ids: "in3", info: "5 Days group page saved" }
                    ]
                },
                {
                    id: "see2", min: "sep2", txt: "Regular", tet: "Recommended for personal pro", amt: "$20", inne: [
                        { ids: "in4", info: "Up to 15 page each group" },
                        { ids: "in5", info: "Download page up to 20 page" },
                        { ids: "in6", info: "Up to 10 group page" },
                        { ids: "in7", info: "15 Days group page saved" }
                    ]
                },
                {
                    id: "see3", min: "sep3", txt: "Premium", tet: "Packet for Startup & Company", amt: "$48", inne: [
                        { ids: "in8", info: "Unlimited group pages" },
                        { ids: "in9", info: "Unlimited download page" },
                        { ids: "in10", info: "Unlimited page each group" },
                        { ids: "in11", info: "Customize sorting group pages" },
                        { ids: "in12", info: "Customize group page name" },
                        { ids: "in13", info: "30 Days group page saved" }
                    ]
                },
            ]
        }
    }
}
</script>

<style scoped>
.pop {
    width: 360px;
    height: 640px;
    background: #FAFAFA;
    border-radius: 16px;
    padding: 32px 32px 24px 32px;
}

h2 {
    height: 64px;
    font-style: normal;
    font-weight: 400;
    font-size: 64px;
    line-height: 100%;
    color: #000000;
}

#hun {
    width: 58px;
    height: 18px;
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 100%;
    color: #000000;
}

#uni {
    padding: 140px;
    background: #000000;
}

#sep2 {
    background: #A8FF35;

}


#sep2 hr {
    opacity: 0.2;
    border: 1px solid #000000;
}

#ion {
    display: flex;
    align-items: baseline;
    padding: 32px 0 32px 0;
}

h1 {
    /* width: 1160px; */
    height: 76px;
    font-style: normal;
    font-weight: 700;
    font-size: 64px;
    line-height: 76px;
    text-align: center;
    color: #FFFFFF;
}

#mont {
    font-style: normal;
    font-weight: 500;
    font-size: 24px;
    line-height: 29px;
    color: #FFFFFF;
}

#yea {
    font-style: normal;
    font-weight: 500;
    font-size: 24px;
    line-height: 29px;
    color: #F5F5F5;
    opacity: 0.5;
}

#vash {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 24px;
    padding-top: 30px;
    padding-bottom: 36px;
}

#cards {
    display: flex;
    gap: 40px;
    flex-wrap: wrap;

}

#popo {
    width: 136px;
    height: 36px;
    font-style: normal;
    font-weight: 400;
    font-size: 36px;
    line-height: 100%;
    color: #000000;
}

#momo {
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 100%;
    /* identical to box height, or 18px */
    padding: 8px 0 32px 0;
    color: #000000;
}

li {
    padding-bottom: 24px;
}

ul {
    list-style: none;
}

ul li:before {
    content: '✓  ';
}
</style>