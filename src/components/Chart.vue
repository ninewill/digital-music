<template>
  <div>
    <canvas id="salaryBar"></canvas>
  </div>
</template>

<script>
export default {
  components: {},
  mounted() {
    var ctx = document.getElementById("salaryBar").getContext("2d");
    Chart.defaults.global.defaultFontColor = "#fff";
    var myChart = new Chart(ctx, {
      //responsive: true,
      //scaleFontColor: "#FFFFFF",
      type: "horizontalBar",
      data: {
        labels: [
          "音樂製作者",
          "杜比環繞",
          "混音師",
          "錄音師",
          "音效製作",
          "微電影音效製作",
          "純音樂編曲",
          "後製配音/配樂",
        ],
        datasets: [
          {
            label: "Votes",
            data: [42, 35, 35, 35, 30, 10, 5, 3],
            backgroundColor: [
              "rgba(255, 159, 64, 2)",
              "rgba(255, 159, 64, 2)",
              "rgba(255, 159, 64, 2)",
              "rgba(255, 159, 64, 2)",
              "rgba(255, 159, 64, 2)",
              "rgba(255, 159, 64, 2)",
              "rgba(255, 159, 64, 2)",
              "rgba(255, 159, 64, 2)",
            ],
						borderWidth: 1,
          },
        ],
      },
      options: {
        legend: {
          display: false,
        },
        scales: {
          xAxes: [
            {
              ticks: {
                beginAtZero: true,
                fontSize: 18,
                max: 45,
                callback: function (value, index, values) {
                  return "$" + value + "K";
                },
              },
            },
          ],
          yAxes: [
            {
							barPercentage: 0.4,
              ticks: {
                beginAtZero: true,
                fontSize: 18,
              },
            },
          ],
        },
      },
    });
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";

#salaryBar {
  width: 100%;
}
</style>