<template>
    <section class="full-width-section">
        <div class="left-side">
            <h1>
                Think bigger.
            </h1>
            <h2>Build faster.</h2>
            <p class="small-text">Figma helps design and development teams build great products, together.</p>
            <button @mouseover="hover = true" @mouseleave="hover = false" @click="showModal = true"
                :class="{ 'hovered': hover }" class="cta-button">
                <span v-if="hover"> → </span>Get started for free
            </button>
        </div>
        <div class="right-side">
            <img src="@/public/Right_animation.png" alt="Animation" />
        </div>

    </section>

    <section>
        <span class="hero">

            <img src="@/public/Hero_Img.png" alt="Hero" />

        </span>
    </section>

</template>


<script>
export default {
    data() {
        return {
            hover: false,
            showModal: false,
        };
    },
};
</script>

<style scoped>
.get-started-animated {
    position: relative;
    transition: transform 0.3s;
}

.get-started-animated:hover {
    transform: scale(1.05);
}

.full-width-section {
    display: flex;
    width: 100%;
    /* margin-bottom: 40px; */
}

.left-side {
    width: 50%;
    padding: 20px;
}

.right-side {
    width: 50%;
}

h1 {
    font-size: 72px;
    /* Большой шрифт */
    line-height: 1.1;
    letter-spacing: -0.0275rem;
    font-weight: 400;
    font-variation-settings: "wdth" 96, "wght" 400;
    margin: 0;
    margin-bottom: 0px;
    color: var(--f-text-color, #000000);
    text-wrap: wrap;
    margin-bottom: 1rem;

}

h2 {
    font-size: 72px;
    /* Большой шрифт */
    line-height: 1.1;
    letter-spacing: -0.0275rem;
    font-weight: 400;
    font-variation-settings: "wdth" 96, "wght" 400;
    margin: 0;
    margin-bottom: 0px;
    color: var(--f-text-color, #000000);
    text-wrap: wrap;
    margin-bottom: 1rem;
}

.small-text {
    font-size: 1.2em;
    /* Меньший шрифт */
}

.cta-button {
    background-color: black;
    color: white;
    border: none;
    border-radius: 25px;
    /* Округлые края */
    padding: 10px 20px;
    cursor: pointer;
    transition: border-radius 0.3s;
}

.cta-button.hovered {
    border-radius: 0;
    /* Прямые края при наведении */
}

.modal {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.7);
    display: flex;
    justify-content: center;
    align-items: center;
}

.modal-content {
    background: white;
    padding: 20px;
    border-radius: 5px;
}

.full-width-section {
    display: flex;
    width: 100%;
}

.large-text {
    font-size: 3em;
    /* Большой шрифт */
}

.small-text {
    font-size: 1.2em;
    /* Меньший шрифт */
}

.cta-button {
    background-color: black;
    color: white;
    border: none;
    border-radius: 25px;
    /* Округлые края */
    padding: 10px 20px;
    cursor: pointer;
    transition: border-radius 0.3s;
}

.cta-button.hovered {
    border-radius: 0;
    /* Прямые края при наведении */
}

.modal {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.7);
    display: flex;
    justify-content: center;
    align-items: center;
}

.modal-content {
    background: white;
    padding: 20px;
    border-radius: 5px;
}

.hero img {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 95%;
    padding-left: 25px;
    padding-right: 20px;
}

.right-side img {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 90%;
    padding-left: 25px;
    padding-right: 20px;
}

.get-started-animated {
    position: relative;
    transition: transform 0.3s;
}

.get-started-animated:hover {
    transform: scale(1.05);
}

.arrow {
    margin-left: 0.5rem;
}
</style>
