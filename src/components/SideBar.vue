<template>
  <aside>
    <div class="top">
      <div class="logo">
        <v-avatar size="100">
          <img src="@/assets/images/person2.jpg" alt="John" />
        </v-avatar>
        <h2>Hello Marta!</h2>
        <h5 class="text-muted">john@gmail.com</h5>
      </div>
      <div class="close" id="close-btn">
        <span class="material-icons-sharp"> close </span>
      </div>
    </div>
    <div class="sidebar">
      <a class="active" href="#">
        <span class="material-icons-sharp">speed</span>
        <h3>Dashboard</h3>
      </a>
      <a href="#">
        <span class="material-icons-sharp">filter_alt</span>
        <h3>Funnels</h3>
      </a>
      <a href="#">
        <span class="material-icons-sharp">insights</span>
        <h3>Channels</h3>
      </a>
      <a href="#">
        <span class="material-icons-sharp">pie_chart</span>
        <h3>Performance</h3>
        <span class="message-count">26</span>
      </a>
      <a href="#">
        <span class="material-icons-sharp">toggle_on</span>
        <h3>Settings</h3>
      </a>
      <a href="#">
        <span class="material-icons-sharp">file_upload</span>
        <h3>Uploads</h3>
      </a>
      <a href="#">
        <span class="material-icons-sharp">logout</span>
        <h3>Logout</h3>
      </a>
    </div>
  </aside>
  <!----------- END OF ASIDE -------->
</template>

<script>
export default {};
</script>
