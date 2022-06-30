<template>
    <div>
        <h1>Join us on email for</h1>
        <h2>more trending topics</h2>
        <but5 ButtonText="Join Now" id="but5"></but5>
    </div>
</template>

<script>
import but5 from "@/components/Button.vue"
export default {
    name: "Joi-ner",
    components: { but5 }
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
    color: #000000;
}

h2 {
    font-style: normal;
    font-weight: 900;
    font-size: 72px;
    line-height: 112%;
    text-align: center;
    color: #87D322;
    margin-bottom: 40px;
}

div {
    background: #A8FF35;
    padding: 160px 300px 140px 300px;
}

#but5 {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    padding: 16px 32px;
    margin-left: auto;
    margin-right: auto;
    gap: 10px;
    width: 180px;
    height: 57px;
    background: #000000;
    border-radius: 40px;
    font-style: normal;
    font-weight: 700;
    font-size: 18px;
    line-height: 140%;
    text-align: center;
    color: #FFFFFF;
}
</style>