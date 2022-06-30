<template>
    <div id="main">
        <div id="mint">

            <span id="side">Findtrend helps you to increase your productivity and reduce your computer's memory load,
            </span>
            <span id="chiq">an application that can fulfill your daily browsing needs.</span>
        </div>
        <div id="rum">
            <h1>Findtrend make +1000 Startup grow</h1>
            <comp></comp>
        </div>
    </div>

</template>

<script>
import comp from "@/components/Belt/Companies.vue"
export default {
    name: "Eins-1",
    components: { comp }
}
</script>

<style scoped>
#main {
    padding: 140px;
}

#mint {
    width: 1160px;
    height: 304px;

    margin-bottom: 280px;
    font-style: normal;
    font-weight: 700;
    font-size: 64px;
    line-height: 76px;
    color: #000000;
}

#chiq {
    color: #ADADAD;
}

h1 {
    height: 76px;
    font-style: normal;
    font-weight: 700;
    font-size: 64px;
    line-height: 76px;
    text-align: center;
    color: #000000;
}

@media screen and (max-width: 375px) {
    #main {
        padding: 80px 18px;
    }



    #mint {
        width: 325px;
        height: 294px;
        margin-bottom: 280px;
        font-style: normal;
        font-weight: 900;
        font-size: 36px;
        line-height: 43px;
        color: #000000;
    }

    h1 {
        width: 335px;
        height: 86px;
        font-style: normal;
        font-weight: 900;
        font-size: 36px;
        line-height: 43px;
        text-align: center;

        color: #000000;
    }
}
</style>