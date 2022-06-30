<template>
    <div id="bore">

        <div id="dance">
            <img src="@/assets/footlogo.svg" alt="">
            <div id="limp">
                <ul v-for="item in fact" :key="item.id">
                    <li><a href="#">{{ item.info }}</a></li>
                </ul>
            </div>
        </div>
    </div>

</template>

<script>
export default {
    name: "Big-foot",
    data() {
        return {
            fact: [
                { id: "fat1", info: "Privacy Policy" },
                { id: "fat1", info: "Terms and Conditions" },
                { id: "fat1", info: "Contact Us" },
                { id: "fat1", info: "Careers" }
            ]
        }
    }
}
</script>

<style scoped>
#bore {
    padding: 28px 100px 28px 80px;
}

#dance {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

#limp {
    display: flex;
    gap: 40px;
}

ul {
    list-style: none;
}

li a {
    text-decoration: none;
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 100%;
    text-align: center;
    color: #000000;
}

@media screen and (max-width: 375px) {
    #bore {
        padding: 0;
    }

    #dance {
        flex-direction: column;
    }

    #limp {
        flex-direction: column;
        align-items: center;
        padding: 98px 0 80px 0;
    }

    img {
        padding-top: 62px;
    }
}
</style>