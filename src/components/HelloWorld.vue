<script>
export default {
  data() {
    return {
      calculatedTime: {
        days: 0,
        hours: 0,
        minutes: 0,
        seconds: 0,
      },
    };
  },
  methods: {
    calculate() {
      const currentDate = new Date();
      const travelDate = new Date("2024-03-25");
      const timeDifference = travelDate - currentDate;

      if (timeDifference > 0) {
        const oneSecond = 1000;
        const oneMinute = oneSecond * 60;
        const oneHour = oneMinute * 60;
        const oneDay = oneHour * 24;

        this.calculatedTime.days = Math.floor(timeDifference / oneDay);
        this.calculatedTime.hours = Math.floor((timeDifference % oneDay) / oneHour);
        this.calculatedTime.minutes = Math.floor((timeDifference % oneHour) / oneMinute);
        this.calculatedTime.seconds = Math.floor((timeDifference % oneMinute) / oneSecond);
      } else {
        this.calculatedTime = {
          days: 0,
          hours: 0,
          minutes: 0,
          seconds: 0,
        };
      }
    },
  },
  mounted() {
    this.calculate(); 

    window.setInterval(() => {
      this.calculate();
    }, 1000);
  },
  props: {
    msg: {
      type: String,
      required: true,
    },
  },
};
</script>



<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      Follow along my travels!
    </h3>
    <h3>
      Countdown until next travel: {{ calculatedTime.days }} days, {{ calculatedTime.hours }} hours, 
      {{ calculatedTime.minutes }} minutes, {{ calculatedTime.seconds }} seconds
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
