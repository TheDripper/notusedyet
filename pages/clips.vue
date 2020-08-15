<template>
  <div class="slide flex flex-col md:flex-row staticbg">
    <div id="sean_monterrosa" class="relative frame">
      <img v-for="src in alt" :src="src" />
    </div>
    <div id="agnes_chow" class="relative frame">
      <img v-for="src in alt" :src="src" />
    </div>
  </div>
</template>
<style lang="scss" scoped>
h1 {
  font-size: 50px;
  z-index: 2;
}
.slide {
  @apply p-2;
  display: flex;
  align-items: center;
  justify-content: center;
  background: black;
}
.frame {
  height: 600px;
  width: 600px;
  overflow: hidden;
  padding: 7px;
  @apply flex items-center justify-center;
}
.copy {
  @apply absolute;
}
#sean_monterrosa {
  background: magenta;
  .copy {
    bottom: 270px;
    left: 0;
  }
  img {
    @apply absolute;
    top: 0;
    left: 0;

    min-height: 100%;
    min-width: 100%;
    max-width: none;
  }
}
#agnes_chow {
  background: cyan;
  margin-left: 20px;
  .copy {
    margin-top: 20px;
  }
  img {
    @apply absolute;
    top: 0;
    left: 0;
    min-height: 100%;
    min-width: 100%;
    max-width: none;
  }
}
.staticbg {
  background-image: url("/static.jpg");
}
</style>
<script>
export default {
  mounted() {
    let black = this.black;
    for (let i = 0; i < black.length; i++) {
      setTimeout(function () {
        black.pop();
      }, i * 1000);
    }
    let white = this.white;
    for (let i = 0; i < white.length; i++) {
      setTimeout(function () {
        white.pop();
      }, i * 1000);
    }
    let alt = this.alt;
    for (let i = 0; i < alt.length; i++) {
      setTimeout(function () {
        alt.pop();
      }, i * 1000);
    }
  },
  data() {
    return {
      alt: [
        "/nike_of_the_mind.png",

        "/nasdaq_fam",
        "/shooting_of_larry_jackson_jr.png",

        "/we_will_stop_this_now.png",
        "/shooting_of_anthony_lamar_smith.png",

        "/we_need_to_stop.png",
        "/shooting_of_trayvon_martin.png",

        "/us_russia_tech_deals.png",
        "/shooting_of_mark_duggan.png",

        "/unicorns_such_rarity.png",
        "/shooting_of_ramarley_graham.png",

        "/salesforce_cartoon_origami_asmr.png",
        "/death_of_kelly_thomas.png",

        "/ruslan_fazlyev_oligarch_putin.png",
        "/shooting_of_anthony_hill.png",

        "/nasdaq_human_heartbeat.png",
        "/shooting_of_timothy_russell_and_malissa_williams.png",

        "/musk_phone.png",
        "/shooting_of_jonathan_ferrell.png",

        "/market_share.png",
        "/shooting_of_john_crawford_iii.png",

        "/thriver_wellness.jpg",
        "/shooting_of_terence_crutcher.png",

        "/bezos_praying_to_money.png",
        "/shooting_of_amadou_diallo.png",

        "/nasdaq_brp.png",
        "/shooting_of_samuel_dubose.png",

        "/nasdaq_adaptive.png",
        "/death_of_freddie_gray.png",

        "/nasdaq_argenx.png",
        "/shooting_of_rekia_boyd.png",

        "/nasdaq_docusign.png",
        "/shooting_of_tamir_rice.png",

        "/nasdaq_funko.png",
        "/shooting_of_sean_bell.png",

        "/nasdaq_tillray.png",
        "/shooting_of_oscar_grant.png",

        "/nasdaq_can.png",
        "/shooting_of_michael_brown.png",

        "/nasdaq_newtek.png",
        "/death_of_eric_garner.png",

        "/nasdaq_blackbaud.png",
        "/death_of_sandra_bland.png",

        "/nasdaq_fluent.png",
        "/shooting_of_walter_scott.png",

        "/nasdaq_pagerduty.png",
        "/shooting_of_philando_castile.png",

        "/nasdaq_lyft.png",
        "/shooting_of_nia_wilson.png",

        "/nasdaq_ruhnn.png",
        "/shooting_of_breonna_taylor.png",
        "/nasdaq_niu.png",
        "/killing_of_george_floyd.png",
        "/nasdaq_longfin.png",
        "/shooting_of_sean_monterrosa.png",
        "/nasdaq_paypal.png",
      ],
      black: [
        "/shooting_of_larry_jackson_jr.png",
        "/shooting_of_anthony_lamar_smith.png",
        "/shooting_of_trayvon_martin.png",
        "/shooting_of_mark_duggan.png",
        "/shooting_of_ramarley_graham.png",
        "/death_of_kelly_thomas.png",
        "/shooting_of_anthony_hill.png",
        "/shooting_of_timothy_russell_and_malissa_williams.png",
        "/shooting_of_jonathan_ferrell.png",
        "/shooting_of_john_crawford_iii.png",
        "/shooting_of_terence_crutcher.png",
        "/shooting_of_amadou_diallo.png",
        "/shooting_of_samuel_dubose.png",
        "/death_of_freddie_gray.png",
        "/shooting_of_rekia_boyd.png",
        "/shooting_of_tamir_rice.png",
        "/shooting_of_sean_bell.png",
        "/shooting_of_oscar_grant.png",
        "/shooting_of_michael_brown.png",
        "/death_of_eric_garner.png",
        "/death_of_sandra_bland.png",
        "/shooting_of_walter_scott.png",
        "/shooting_of_philando_castile.png",
        "/shooting_of_nia_wilson.png",
        "/shooting_of_breonna_taylor.png",
        "/killing_of_george_floyd.png",
        "/shooting_of_sean_monterrosa.png",
      ],
      white: [
        "/nike_of_the_mind.png",
        "/nasdaq_fam",
        "/we_will_stop_this_now.png",
        "/we_need_to_stop.png",
        "/us_russia_tech_deals.png",
        "/unicorns_such_rarity.png",
        "/salesforce_cartoon_origami_asmr.png",
        "/ruslan_fazlyev_oligarch_putin.png",
        "/nasdaq_human_heartbeat.png",
        "/musk_phone.png",
        "/market_share.png",
        "/thriver_wellness.jpg",
        "/bezos_praying_to_money.png",
        "/nasdaq_brp.png",
        "/nasdaq_adaptive.png",
        "/nasdaq_argenx.png",
        "/nasdaq_docusign.png",
        "/nasdaq_funko.png",
        "/nasdaq_tillray.png",
        "/nasdaq_can.png",
        "/nasdaq_newtek.png",
        "/nasdaq_blackbaud.png",
        "/nasdaq_fluent.png",
        "/nasdaq_pagerduty.png",
        "/nasdaq_lyft.png",
        "/nasdaq_ruhnn.png",
        "/nasdaq_niu.png",
        "/nasdaq_longfin.png",
        "/nasdaq_paypal.png",
      ],
    };
  },
};
</script>