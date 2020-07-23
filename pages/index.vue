<template>
  
  <div class="tile is-ancestor">
  <div class="tile is-4 is-vertical is-parent">
    <nuxt-link to="/RCA" class="tile is-child box has-text-centered notification is-success">
      <p class="title is-1">RCA</p>
      <!-- <Dose /> -->
    </nuxt-link>
    <div class="tile is-child box notification is-warning">
      <p class="title is-1">Heparin</p>
      <p>brief heparin intro</p>
    </div>
  </div>
  <div class="tile is-parent">
    <div class="tile is-child box has-text-centered">
      
      
       <Logo />
    </div>
  </div>
   <div class="tile is-4 is-vertical is-parent">
    <div class="tile is-child box notification is-info">
      <p class="title is-1">No anticoagulation</p>
      <p>brief no anti coag intro</p>
    </div>
    <div class="tile is-child box notification is-danger">
      <p class="title is-1">Advanced Modes</p>
      <p>
        <ul>
          <li>HVHF</li>
          <li>PIRRT</li>
          <li>IHD</li>
        </ul>
      </p>
      <p>These modes should only be started with consultant approval</p>
    </div>
  </div>
</div>
  

 



</template>




<script>
export default {
  layout: 'default_app',
  
  
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}


.links {
  padding-top: 15px;
}
</style>
