<template>
  <div>
    <div class="navbar">
      <div class="nav-item">
        <a class="active" href="#">
          <span>Overview</span>
        </a>
        <a href="#">
          <span>Account 1</span>
        </a>
        <a href="#">
          <span>Account 2</span>
        </a>
      </div>
    </div>
    <insights-component />
    <update-component />
  </div>
</template>

<script>
import InsightsComponent from "./InsightsComponent.vue";
import UpdateComponent from "./UpdateComponent.vue";
export default {
  components: { InsightsComponent, UpdateComponent },
};
</script>

<style>
</style>