<template>
    <button>{{ ButtonText }}</button>
</template>

<script>
export default {
    name: "But-ton",
    props: ["ButtonText"]
}
</script>

<style scoped>
#but1 {
    padding: 12px 32px;
    border-radius: 40px;
}

#but2 {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    padding: 16px 32px;
    gap: 10px;
    width: 180px;
    height: 57px;
    background: #A8FF35;
    border-radius: 40px;
}

#but3 {
    display: block;
    padding: 16px 32px;
    gap: 10px;
    color: white;
    height: 57px;
    background: #000000;
    border-radius: 40px;
    margin-top: 80px;
    margin-left: auto;
    margin-right: auto;
    font-weight: 700;
    font-size: 18px;
    line-height: 140%;
}

#see1,
#see3 {
    width: 296px;
    height: 58px;
    border: none;
    background: #A8FF35;
    border-radius: 29px;
    font-style: normal;
    font-weight: 700;
    font-size: 18px;
    line-height: 140%;
    text-align: center;
    color: #000000;
    margin-top: 160px;

}

#see3 {
    margin-top: 16px;
}

#see2 {
    width: 296px;
    height: 58px;
    background-color: #000000;
    border-radius: 29px;
    font-style: normal;
    font-weight: 700;
    font-size: 18px;
    line-height: 140%;
    text-align: center;
    color: #FFFFFF;
    margin-top: 112px;
}

@media screen and (max-width: 375px) {
    #but2 {
        padding: 12px 24px;
        width: 139px;
        height: 44px;
    }
}
</style>