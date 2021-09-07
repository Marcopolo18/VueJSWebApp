<template>
  <div id="app">
  
  <!-- html files go here --> 
    <div id="content">
        <h1>{{ title }}</h1> 
        <h1 id="h3">{{ date1 }}</h1>

      <ul class="parent">
        
        <li class="list-1">
          <div class="child-1">
            <strong class="time">14:00 Uhr</strong><br>
            <strong class="visitor">Basisbeschäftigung Besuch</strong>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
          </div>
        </li>
      

        <li class="list-2">
          <div class="child-2">
            <strong class="time">14:00 Uhr</strong><br>
            <strong class="visitor">Basisbeschäftigung Besuch</strong>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
          </div>
        </li>
      

        <li class="list-3">
          <div class="child-3">
            <strong class="time">14:00 Uhr</strong><br>
            <strong class="visitor">Basisbeschäftigung Besuch</strong>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
          </div>
        </li>  
      </ul>        

      <footer>
        <div class="image-1"> <img src="./assets/Opportunity.png" width="300%" height="auto"></div>
        <div class="image-2"> <img src="./assets/SAG_Logo_De.png" width="100%" height="auto"></div>
        <div class="image-3"> <img src="./assets/STZH_SEB_Logo.png" width="100%" height="auto"></div>
      </footer>  

    </div>  

  </div>

</template>

<script>

export default {
  name: 'App',
  data() {
    return {
        title: "Welcome to Opportunity",
        date1: "08.08.2021",
        
        };
    }
}
</script>

<style>
/* css styles go here */

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;  
  background-color: rgb(210, 235, 243);  
  height: 1920px;
  width: 1080px; 
  display:flex; 
  margin: 0;
  padding: 0; 
  border: darkblue solid 2px;   
}

#content {
  display: flex;
  flex-direction: column;
  flex-flow: column;
  flex-wrap: wrap;
  font-size: 40px;
  position: relative;  
  align-content: left;
}

p {
  margin: 0;
}

.parent {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  font-size: 32px;
  margin-top: 50px;
  justify-content: center;
  position: relative;
  padding-left: 1%;
  padding-right: 4%;
     
}

.child-1, .child-2, .child-3 {
  background-color: darkblue;      
  width: 960px;   
  padding: 2%;
  margin: 10px;
  border: rgb(99, 96, 250) outset 3px;
  text-align: left;
  line-height: 1.5em;   
}

.time {
  color:rgb(206, 86, 86);
}

.visitor {
  color: rgb(243, 169, 140);
}

p {
  color: rgb(231, 148, 115);
}

footer {
  background-color: white;
  height: 150px;
  width: 1080px;
  display: flex;
  flex-direction: row;  
  justify-content: space-between;
  margin-top: 851px; 
}

.image-1, .image-2, .image-3 {  
  padding: 30px;
  margin: 30px;
}

.image-2, .image-3 {
  margin-left: 100px;
}

li, ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

h1 {
  margin: 10px;
  padding: 0; 
  padding-right: 3%;
  padding-left: 5%; 
  margin-top: 50px;
  
}

#h3 {
  color: gray;
  text-align: left;
  margin: 0;
  padding: 0; 
  padding-right: 3%;
  padding-left: 6%;
  font-weight: normal;
  
}

#app.this.title {
  color: yellow;
}
</style>
