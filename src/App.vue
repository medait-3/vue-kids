 <template>
  <div id="app">
    <img src="./assets/logo.png">
    <form >
      <label>put yuor color:</label>
    <input type="text" v-on:input="cssClass = $event.target.value">
    <h3 style="line-height: 0;font-size: 26px;margin-left: 76%;">  لوني </h3>   
      
    <h3 style="margin-left: 50%" v-if="cssClass === 'yellow'">
الأصفر    </h3>
    <h3 style="margin-left: 50%" v-else-if="cssClass === 'red'">
أحمر    </h3>
    <h3 style="margin-left: 50%" v-else-if="cssClass === 'green'">
أخضر    </h3>
    <h3 style="margin-left: 50%" v-else-if="cssClass === 'grey'">
الرمادي    </h3>
    <h3 style="margin-left: 50%" v-else-if="cssClass === 'black'">
أسود    </h3>
    <h3 style="margin-left: 50%" v-else-if="cssClass === 'pink'">
زهري    </h3>
    <h3 style="margin-left: 50%" v-else-if="cssClass === 'blue'">
أزرق    </h3>
    <h3 style="margin-left: 50%" v-else-if="cssClass === 'orange'">
البرتقالي    </h3>
    <h3 style="margin-left: 50%" v-else-if="cssClass === 'purple'">
أرجواني    </h3>
    <h3 style="margin-left: 50%" v-else-if="cssClass === 'white'">
أبيض    </h3>
    <h3 style="margin-left: 50%" v-else-if="cssClass === 'brown'">
بنى    </h3>

  


    <h2 v-bind:class="cssClass">{{ box }}</h2>

    <h3  v-if="cssClass === 'yellow'">
      <img src="./assets/yellow.jpg">
    </h3>
    <h3 v-else-if="cssClass === 'red'">
      <img src="./assets/red.jpg">
    </h3>
    <h3 v-else-if="cssClass === 'green'">
      <img src="./assets/green.jpg">
    </h3>
    <h3 v-else-if="cssClass === 'grey'">
      <img src="./assets/grey.jpg">
    </h3>
    <h3 v-else-if="cssClass === 'black'">
      <img src="./assets/black.jpg">
    </h3>
    <h3 v-else-if="cssClass === 'pink'">
      <img src="./assets/pink.jpg">
    </h3>
    <h3 v-else-if="cssClass === 'blue'">
      <img src="./assets/blue.jpg">
    </h3>
    <h3 v-else-if="cssClass === 'orange'">
      <img src="./assets/orange.jpg">
    </h3>
    <h3 v-else-if="cssClass === 'purple'">
      <img src="./assets/purple.jpg">
    </h3>
    <h3 v-else-if="cssClass === 'white'">
      <img src="./assets/white.jpg">
    </h3>
    <h3 v-else-if="cssClass === 'brown'">
      <img src="./assets/brown.jpg">
    </h3>
        </form>

  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      cssClass:'',
      box:'',

    }
  }
}
</script>

<style>
  p{padding: 1%;
   margin-left: auto;
  margin-right: auto;
text-align: center;}
 form{
    padding: 1%;
    width: 50%;

  }img {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 200px;
}
input{  width: 190px;
  border-radius: 20%;
  text-align: center;
}
form {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 200px;
}
label{line-height: 4;
  text-align: center;
}
 
  h2{
  width: 90px;
    border-radius: 10%;
  padding: 50px;
  margin: auto;
  border: 1px solid black
  }
.red{
  background-color: red;
}.yellow{
  background-color: yellow;
}.green{
  background-color: green;
}.grey{
  background-color: grey;
}.black{
  background-color: black;
}.pink{
  background-color: #FF1493;
}.blue{
  background-color: #00BFFF;
}.orange{
  background-color: orange;
}.purple{
  background-color: purple;
}.white{
  background-color: white;
}.brown{
  background-color: #A52A2A;
}
</style>
