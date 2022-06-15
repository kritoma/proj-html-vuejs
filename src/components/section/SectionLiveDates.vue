<template>
  <section>
    <div class="container">
        <div class="live">
            <TitleSection title="Live Dates"/>
            <CardDates class="list" v-for="(live, index) in liveDates" :key="index" :live="live"/>
        </div>
    </div>
    <DisplayBar text="VIEW ALL LIVES DATES"/>
  </section>
</template>

<script>
import CardDates from '../common/CardDates.vue';
import DisplayBar from '../common/DisplayBar.vue';
import TitleSection from '../common/TitleSection.vue';

export default {
  components: { TitleSection, CardDates, DisplayBar },
    name: "SectionLiveDates",

    data() {
        return {
            liveDates: [
                {
                    date: "17/08/2020",
                    festival: "GEM FESTIVAL 2020 ANAKALIA",
                    country: "GEORGIA",
                },
                 {
                    date: "24/09/2020",
                    festival: "GROOVEFEST",
                    country: "DOMINICAL REPUBLIC",
                },
                 {
                    date: "31/10/2020",
                    festival: "OASIS FESTIVAL 2020 MARRAKECH",
                    country: "MOROCCO",
                },
                 {
                    date: "07/11/2020",
                    festival: "MOGA FESTIVAL - ESSAOURIA",
                    country: "MOROCCO",
                },
                 {
                    date: "10/12/2020",
                    festival: "ENVISION FESTIVAL - UVITA",
                    country: "COSTA RICA",
                },
            ],
        }
    }
} 
</script>

<style lang="scss" scoped>
section {
    background-color: #252a33;

    .live {
        padding: 5rem 0;
    }


    .list {
        margin: .625rem 0;

    }
    
}
</style>