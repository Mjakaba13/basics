<template>
    <div id="meat">
        <div>
            <img src="@/assets/logo-mob.svg" alt="">
        </div>
        <button id="ham"><img src="@/assets/Ham-mob.svg" alt=""></button>
    </div>
    <div id="nice">
        <div>
            <img src="@/assets/Logo.svg" alt="">
        </div>
        <div id="nicer">
            <ul>
                <li v-for="item in lnk1" :key="item.id">
                    <a href="#">{{ item.iden }}</a>
                </li>
            </ul>
        </div>
        <div id="niced">
            <ul>
                <li><a href="#">Login</a></li>
            </ul>
            <but1 ButtonText="Register" id="but1"></but1>
        </div>
    </div>
</template>

<script>
import but1 from "@/components/Button.vue"
export default {
    name: "Nav-bar",
    components: { but1 },
    data() {
        return {
            lnk1: [
                { id: "l1", iden: "About" },
                { id: "l2", iden: "How it work" },
                { id: "l3", iden: "Pricing" },
                { id: "l4", iden: "Solution" },
                { id: "l5", iden: "Features" }
            ]
        }
    }
}
</script>

<style scoped>
#meat {
    display: none;
}

#nice {
    display: flex;
    align-items: center;
    padding: 38px 60px;
}

ul {
    list-style: none;

}

#nicer {
    padding-left: 210px;
    padding-right: 160px;
}

#nicer ul {
    display: flex;
    gap: 35px;
}

li a {
    text-decoration: none;
    height: 18px;
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 100%;
    text-align: center;

    color: #FFFFFF;
}


#niced {
    display: flex;
    align-items: center;
    gap: 40px;
}

@media screen and (max-width: 375px) {
    #meat {
        display: block;
        padding: 24px 18px;
        display: flex;
        justify-content: space-between;
    }

    #nice {
        display: none;
    }

    #ham {
        background-color: black;
        border: none;
    }
}
</style>