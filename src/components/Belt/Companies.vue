<template>
    <div id="mant">

        <div id="fatt" v-for="item in pics" :key="item.id">
            <img :src="item.imgg" alt="">
        </div>
    </div>
</template>

<script>
export default {
    name: "Comp-anies",

    data() {
        return {
            pics: [
                { id: "p1", imgg: require("@/assets/Microsoft.svg") },
                { id: "p2", imgg: require("@/assets/Allianz.svg") },
                { id: "p3", imgg: require("@/assets/Upwork.svg") },
                { id: "p4", imgg: require("@/assets/Volvo.svg") },
                { id: "p5", imgg: require("@/assets/Grab.svg") },
                { id: "p6", imgg: require("@/assets/Verizon.svg") },
                { id: "p7", imgg: require("@/assets/coinbase.svg") },
                { id: "p8", imgg: require("@/assets/Expedia.svg") },
                { id: "p8", imgg: require("@/assets/Airtable.svg") },
                { id: "p8", imgg: require("@/assets/Magento.svg") },
                { id: "p8", imgg: require("@/assets/Carrera.svg") },
                { id: "p8", imgg: require("@/assets/Bonanza.svg") },
                { id: "p8", imgg: require("@/assets/Wetransfer.svg") },
                { id: "p8", imgg: require("@/assets/Suzuki.svg") },
                { id: "p8", imgg: require("@/assets/Algolia.svg") },
                { id: "p8", imgg: require("@/assets/Heineken.svg") }
            ]
        }
    }
}
</script>

<style scoped>
#mant {
    padding-top: 80px;
    display: flex;
    flex-wrap: wrap;
    row-gap: 32px;
    column-gap: 32px;
}

#fatt {
    width: 242px;
    height: 120px;
    left: 736px;
    top: 2522px;
    padding: 42px 32px;
    background: #F5F5F5;
    border-radius: 8px;
}

@media screen and (max-width: 375px) {
    #mant {
        justify-content: center;
    }
}
</style>