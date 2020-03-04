<template>
  <div class="hello bg-light">
      <!-- This class contains the landing page    -->
      <div class="content">
        <div class="landing-text">
        <h1>Your <strong style="color:gold">IDEA</strong> Goes Here</h1>
        <h4>
          Lorem ipsum dolor sit, amet consectetur 
          elit. Incidunt veritatis sint eos! 
          Fugiat ducimus  
        </h4>
        <div class="landing-buttons mt-4">
          <button class="btn btn-light btn-lg mr-3" type="submit">BROWSE FOR IDEAS</button>
          <button class="btn btn-warning btn-lg" type="submit">YOUR IDEA</button>
        </div>
      </div>
      <div class="landing-image">
        <img src="../assets/landing-2.png" class="img-fluid" alt="" />
      </div>
      </div>
      <!-- scroll animation -->
      <div class="icon-scroll" target=".category"></div>
  </div>
  
</template>

<script>
export default {
  name: 'HelloWorld',
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.content{
  height: 100vh;
  display: flex;
  align-items: center;
  text-align: center;
  
}

.landing-text h1{
  font-size: 55px;
}

.landing-image{
  width: 50%;
}

.landing-text{
  width: 50%;
  text-align: center;
  padding: 20px;
}

.icon-scroll,
.icon-scroll:before{
  position: absolute;
  left: 50%
}

.icon-scroll{
  clear: both;
  width: 40px;
  height: 70px;
  bottom: 10px;
  box-shadow: inset 0 0 0 1px gold;
  border-radius: 25px;
}

.icon-scroll:before{
  content: '';
  width: 8px;
  height: 8px;
  background: gold;
  margin-left: -4px;
  top: 8px;
  border-radius: 4px;
  animation-duration: 1.5s;
  animation-iteration-count: infinite;
  animation-name: scroll;
}

@keyframes scroll{
  0%{
    opacity: 1;}
  100%{  
    opacity: 0;   
    transform: translateY(46px);}
}

</style>
