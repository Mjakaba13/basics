<template>
    <div id="meat">
        <div id="gun">
            <img src="@/assets/logo-mob.svg" alt="">
        </div>
        <button id="ham" v-on:click="displayMenu"><img class="open" :class="[toggle ? open2 : '']"
                src="@/assets/Ham-mob.svg" alt=""><img :class="[toggle ? close2 : '']" class="close"
                src="@/assets/closeicon.svg"></button>
    </div>
    <div class="nice" :class="[toggle ? linkhidder : '']">
        <div id="nices">
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
        <div class="overlay"></div>
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
            ],
            toggle: false,
            close2: 'close2',
            open2: 'open2',
            linkhidder: 'linkhidder'

        }
    },
    methods: {
        displayMenu() {
            this.toggle = !this.toggle

        }
    }
}
</script>

<style scoped>
#meat {
    display: none;
}

.nice {
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

    #gun {
        z-index: 3;

    }

    #nices {
        display: none;
    }

    #ham {
        background-color: black;
        border: none;
        /* right: 18px;
        position: absolute; */
        z-index: 2;
    }

    .close {
        display: none;

    }

    .close2 {
        display: block;
    }

    .open2 {
        display: none;
    }

    .nice {
        display: none;
    }

    #nicer {
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 0;

    }

    #nicer ul {
        align-items: center;
    }

    #nicer ul,
    #niced {
        flex-direction: column;
    }

    #niced {
        margin-top: 40px;
    }

    .linkhidder {
        display: block;
        position: absolute;
        z-index: 1;
        background-color: black;
        width: 100%;
    }

    .overlay {
        height: 100%;
        width: 100%;
        position: fixed;
        background-color: black;
        opacity: 0.5;
        bottom: 0;
        z-index: -1;
        left: 0;
    }
}
</style>