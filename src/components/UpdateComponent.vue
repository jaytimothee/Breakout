<template>
  <div class="right">
    <div class="top">
      <button id="menu-btn">
        <span class="material-icons-sharp">menu</span>
      </button>
      <div class="theme-toggler">
        <span class="material-icons-sharp active">light_mode</span>
        <span class="material-icons-sharp">dark_mode</span>
      </div>
    </div>
    <!---------- END OF TOP ------------------>
    <div>
        <h2>Monthly Analysis</h2>
      <v-sparkline
        :fill="fill"
        :gradient="selectedGradient"
        :line-width="width"
        :padding="padding"
        :smooth="radius || false"
        :value="value"
        auto-draw
      ></v-sparkline>
    </div>
    <!------------- END OF UPDATES -------------->
    <div class="sales-analytics">
      <h2>User Analytics</h2>
      <div class="item online">
        <div class="icon">
          <span class="material-icons-sharp active">receipt_long</span>
        </div>
        <div class="right">
          <div class="info">
            <h3>POST</h3>
            <small class="text-muted">Last 24 Hours</small>
          </div>
          <h5 class="success">+39%</h5>
          <h3>3849</h3>
        </div>
      </div>
      <div class="item offline">
        <div class="icon">
          <span class="material-icons-sharp active">favorite</span>
        </div>
        <div class="right">
          <div class="info">
            <h3>COMMENTS</h3>
            <small class="text-muted">Last 24 Hours</small>
          </div>
          <h5 class="danger">-17%</h5>
          <h3>234</h3>
        </div>
      </div>
      <div class="item customers">
        <div class="icon">
          <span class="material-icons-sharp active">photo_camera</span>
        </div>
        <div class="right">
          <div class="info">
            <h3>UPLOADS</h3>
            <small class="text-muted">Last 24 Hours</small>
          </div>
          <h5 class="success">+25%</h5>
          <h3>865</h3>
        </div>
      </div>
      <div class="item add-product">
        <div>
          <span class="material-icons-sharp">add</span>
          <h3>BOOST CAMPAIGN</h3>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
const gradients = [
  ["#7380ec","#41f1b6", "#dce1eb" ],
  ["#42b3f4"],
  ["red", "orange", "yellow"],
  ["purple", "violet"],
  ["#00c6ff", "#F0F", "#FF0"],
  ["#f72047", "#ffd200", "#1feaea"],
];

export default {
  data: () => ({
    fill: true,
    selectedGradient: gradients[0],
    gradients,
    padding: 8,
    radius: 10,
    value: [0, 2, 5, 9, 5, 10, 3, 5, 0, 0, 1, 8, 2, 9, 0],
    width: 2,
  }),
};
</script>

<style>
</style>