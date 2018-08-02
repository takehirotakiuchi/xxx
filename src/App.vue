<template>
<div id="app">
  <div class="block">
    <span class="demonstration">星座占い🔮</span>
    <el-date-picker
      v-model="value1"
      type="date"
      placeholder="占い">
    </el-date-picker>
    <button v-on:click='Uranai'>占う🔮</button>
  </div>
  <div v-for='Horoscope in  Horoscopes' id="container" v-if='show'>
    <div id="con_left">
      <h1>{{ Horoscope.name }}</h1>
      <h2>総合点{{  Horoscope.point }}</h2>
      <p>{{  Horoscope.desciption }}</p>
      <table class="table">
      <tr>
      <th>今日のラッキーカラー</th>
      <td>{{ Horoscope.color }}</td>
      </tr>
      <tr>
      <th>今日のラッキーアイテム</th>
      <td>{{ Horoscope.item }}</td>
      </tr>
      </table>
    </div>
    <div id="con_right">
      <h3>恋愛運</h3>
      <p>{{  Horoscope.love }}</p>
      <h3>金銭運</h3>
      <p>{{  Horoscope.work }}</p>
      <h3>仕事運</h3>  
      <p>{{  Horoscope.money }}</p>
    </div>
   </div> 
  </div>
</div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import axios from 'axios'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  mounted(){
  for(var i = 0; i < 12; i++){
    this.Horoscopes.push(
         {
          name:'',
          point:'',
          desciption:'',
          color:'',
          item:'',
          love:'',
          work:'',
          moeny:'',
        }
      )
  }
  },
  data(){
    return {
      show:false,
      value1:'',
      Horoscopes:[],
      names: [
        'Aquarius',
        'Aries',
        'Cancer',
        'Capricorn',
        'Gemini',
        'Leo',
        'Libra',
        'Pisces',
        'Sagittarius',
        'Scorpius',
        'Taurus',
        'Virgo'
      ]
    }
  },
  methods:{
    Uranai:function(){
      this.show = true;
      for(let index = 0; index < this.names.length; index++) {
      axios.get(`/static/json/${this.names[index]}.json`).then((e) => { 
     this.Horoscopes[index].name = e.data.name
      this.Horoscopes[index]={
        name:e.data.name,
        point:e.data.point,
        desciption:e.data.desciption,
        color:e.data.color,
        item:e.data.item,
        love:e.data.love,
        work:e.data.work,
        moeny:e.data.moeny
          }
        });
      }
    }
  }
}
</script>


<style>

body {
  background-image: linear-gradient(135deg, #fdfcfb 0%, #e2d1c3 100%);
  background-attachment: fixed;
  height: 100vh;
}

.block{
  margin: 2em 0;
  text-align: center;
}

  *{
    padding: 0;
    margin: 0;
    list-style-type: none;
  }

  h1,
  h2{
    text-align: center;
  }

  h3{
    border-left: 3px solid #000000;
    border-bottom: 1px solid #000000;
    margin-bottom: 0.5em;
    padding-left: 0.3em;
  }

  td,
  th{
    border: solid 1px #000000;
  }

  th{
    /* background-color: blue; */
  }

  table{
    margin-top: 2em;
  }
  
  #container{
    width: 900px;
    margin: 0 auto;
    overflow: hidden;
    padding: 1em;
    box-shadow: 6px 6px;
    margin-bottom: 4em;
    background-image: linear-gradient(to top, #a8edea 0%, #fed6e3 100%);
  }

  #con_left,
  #con_right{
    width: 400px;
    box-sizing :border-box;
  }

  #con_left{
    float: left;
    margin-right: 2em;
  }

  #con_right{
    overflow: hidden;
  }

  .table{
    border: solid 1px #ffffff; 
    border-collapse: collapse;
    text-align: left;
  }

  #con_right p{
      margin-bottom: 1em;
  }


</style>
