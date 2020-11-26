<template>
    <section class="mw" id="explanation">
        <div class="top">
            <h2>{{ title_top }}</h2>
            <p>{{ message_top }}</p>
        </div>
        <div class="bottom">
            <h2>{{ title_bottom }}</h2>
            <p>{{ message_bottom }}</p>
        </div>
    </section>
</template>


<script>
export default {
    name: "Explanation",
    data: function () {
        return {
            title_top: "Parkeercapaciteit: op elk moment van elke dag.",
            message_top: "Om inzicht te geven in het aantal parkeerplaatsen in Nederlandse plaatsen is het parkeercapaciteit-platform ontwikkeld: een informatieve web app gericht op Nederlandse steden en dorpen. Het aantal parkeerplaatsen wordt visueel weergegeven in de vorm van een interactieve bar chart en toont data van alle gemeentes waarvan dit beschikbaar is.",
            title_bottom: "Interactieve barchart",
            message_bottom: "In de onderstaande barchart zijn een aantal input fields. Bovenin kun je kiezen of je het aantal parkeerplaatsen wil bekijken in getallen of in procenten. Hiernaast, bij 'Dag' kun je de dag van de week selecteren. Bij 'Tijd' kun je bepalen op welk moment van de dag je de parkeercapaciteit wil bekijken. Vervolgens kun je bij 'Gemeentes' alle steden of dorpen selecteren die je in de staafdiagram wil visualiseren."
        }
    }
}
</script>


<style scoped>
    .mw h2 {font-size: 2rem; font-family: "Bebas Neue"; margin-left: 0;}
    .top { margin-top: 4rem;}
    p {margin-bottom: 0.6rem; max-width: 35rem; font-size: 0.8rem;}
    
    .bottom {text-align: right; margin: 4rem 2rem 8rem; }
    .bottom p {margin-left: auto;}

    @media only screen and (max-width: 800px) {
        .mw h2 { font-size: 1.2rem;}
        .bottom {text-align: left;}
        .mw > div { margin: 1rem;}
        div.top {margin-top: 4rem;}
    }
</style>