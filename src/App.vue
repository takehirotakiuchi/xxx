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
    <div id="container" v-if="show">
      <div id="con_left">
        <h1>{{ name }}</h1>
        <h2>総合運{{ point }}</h2>
        <p>{{ desciption }}</p>
        <table class="table">
          <tr>
            <th>今日のラッキーカラー</th>
            <td>{{ color }}</td>
          </tr>
          <tr>
            <th>今日のラッキーアイテム</th>
            <td>{{ item }}</td>
          </tr>
        </table>
      </div>
      <div id="con_right">
        <h3>恋愛運</h3>
        <p>{{ love }}</p>
        <h3>金銭運</h3>
        <p>{{ moeny }}</p>
        <h3>仕事運</h3>
        <p>{{ work }}</p>
      </div>
    </div>
     <div id="container" v-if='show'>
      <div id="con_left">
        <h1>{{ name2 }}</h1>
        <h2>総合運{{ point2 }}</h2>
        <p>{{ desciption2 }}</p>
        <table class="table">
          <tr>
            <th>今日のラッキーカラー</th>
            <td>{{ color2 }}</td>
          </tr>
          <tr>
            <th>今日のラッキーアイテム</th>
            <td>{{ item2 }}</td>
          </tr>
        </table>
      </div>
      <div id="con_right">
        <h3>恋愛運</h3>
        <p>{{ love2 }}</p>
        <h3>金銭運</h3>
        <p>{{ moeny2 }}</p>
        <h3>仕事運</h3>
        <p>{{ work2 }}</p>
      </div>
    </div>
     <div id="container" v-if='show'>
      <div id="con_left">
        <h1>{{ name3 }}</h1>
        <h2>総合運{{ point3 }}</h2>
        <p>{{ desciption3 }}</p>
        <table class="table">
          <tr>
            <th>今日のラッキーカラー</th>
            <td>{{ color3 }}</td>
          </tr>
          <tr>
            <th>今日のラッキーアイテム</th>
            <td>{{ item3 }}</td>
          </tr>
        </table>
      </div>
      <div id="con_right">
        <h3>恋愛運</h3>
        <p>{{ love3 }}</p>
        <h3>金銭運</h3>
        <p>{{ moeny3 }}</p>
        <h3>仕事運</h3>
        <p>{{ work3 }}</p>
      </div>
    </div>
     <div id="container" v-if='show'>
      <div id="con_left">
        <h1>{{ name4 }}</h1>
        <h2>総合運{{ point4 }}</h2>
        <p>{{ desciption4 }}</p>
        <table class="table">
          <tr>
            <th>今日のラッキーカラー</th>
            <td>{{ color4 }}</td>
          </tr>
          <tr>
            <th>今日のラッキーアイテム</th>
            <td>{{ item4 }}</td>
          </tr>
        </table>
      </div>
      <div id="con_right">
        <h3>恋愛運</h3>
        <p>{{ love4 }}</p>
        <h3>金銭運</h3>
        <p>{{ moeny4 }}</p>
        <h3>仕事運</h3>
        <p>{{ work4 }}</p>
      </div>
    </div>
    <div id="container" v-if='show'>
      <div id="con_left">
        <h1>{{ name5 }}</h1>
        <h2>総合運{{ point5 }}</h2>
        <p>{{ desciption5 }}</p>
        <table class="table">
          <tr>
            <th>今日のラッキーカラー</th>
            <td>{{ color5 }}</td>
          </tr>
          <tr>
            <th>今日のラッキーアイテム</th>
            <td>{{ item5 }}</td>
          </tr>
        </table>
      </div>
      <div id="con_right">
        <h3>恋愛運</h3>
        <p>{{ love5 }}</p>
        <h3>金銭運</h3>
        <p>{{ moeny5 }}</p>
        <h3>仕事運</h3>
        <p>{{ work5 }}</p>
      </div>
    </div>
     <div id="container" v-if='show'>
      <div id="con_left">
        <h1>{{ name6 }}</h1>
        <h2>総合運{{ point6 }}</h2>
        <p>{{ desciption6 }}</p>
        <table class="table">
          <tr>
            <th>今日のラッキーカラー</th>
            <td>{{ color6 }}</td>
          </tr>
          <tr>
            <th>今日のラッキーアイテム</th>
            <td>{{ item6 }}</td>
          </tr>
        </table>
      </div>
      <div id="con_right">
        <h3>恋愛運</h3>
        <p>{{ love6}}</p>
        <h3>金銭運</h3>
        <p>{{ moeny6 }}</p>
        <h3>仕事運</h3>
        <p>{{ work6 }}</p>
      </div>
    </div>
    <div id="container" v-if='show'>
      <div id="con_left">
        <h1>{{ name7 }}</h1>
        <h2>総合運{{ point7 }}</h2>
        <p>{{ desciption7 }}</p>
        <table class="table">
          <tr>
            <th>今日のラッキーカラー</th>
            <td>{{ color7 }}</td>
          </tr>
          <tr>
            <th>今日のラッキーアイテム</th>
            <td>{{ item7 }}</td>
          </tr>
        </table>
      </div>
      <div id="con_right">
        <h3>恋愛運</h3>
        <p>{{ love7}}</p>
        <h3>金銭運</h3>
        <p>{{ moeny7 }}</p>
        <h3>仕事運</h3>
        <p>{{ work7 }}</p>
      </div>
    </div>
    <div id="container" v-if='show'>
      <div id="con_left">
        <h1>{{ name8 }}</h1>
        <h2>総合運{{ point8 }}</h2>
        <p>{{ desciption8 }}</p>
        <table class="table">
          <tr>
            <th>今日のラッキーカラー</th>
            <td>{{ color8 }}</td>
          </tr>
          <tr>
            <th>今日のラッキーアイテム</th>
            <td>{{ item8 }}</td>
          </tr>
        </table>
      </div>
      <div id="con_right">
        <h3>恋愛運</h3>
        <p>{{ love8}}</p>
        <h3>金銭運</h3>
        <p>{{ moeny8 }}</p>
        <h3>仕事運</h3>
        <p>{{ work8 }}</p>
      </div>
    </div>
    <div id="container" v-if='show'>
      <div id="con_left">
        <h1>{{ name9 }}</h1>
        <h2>総合運{{ point9 }}</h2>
        <p>{{ desciption9 }}</p>
        <table class="table">
          <tr>
            <th>今日のラッキーカラー</th>
            <td>{{ color9 }}</td>
          </tr>
          <tr>
            <th>今日のラッキーアイテム</th>
            <td>{{ item9 }}</td>
          </tr>
        </table>
      </div>
      <div id="con_right">
        <h3>恋愛運</h3>
        <p>{{ love9}}</p>
        <h3>金銭運</h3>
        <p>{{ moeny9 }}</p>
        <h3>仕事運</h3>
        <p>{{ work9 }}</p>
      </div>
    </div>
    <div id="container" v-if='show'>
      <div id="con_left">
        <h1>{{ name10 }}</h1>
        <h2>総合運{{ point10 }}</h2>
        <p>{{ desciption10 }}</p>
        <table class="table">
          <tr>
            <th>今日のラッキーカラー</th>
            <td>{{ color10 }}</td>
          </tr>
          <tr>
            <th>今日のラッキーアイテム</th>
            <td>{{ item10 }}</td>
          </tr>
        </table>
      </div>
      <div id="con_right">
        <h3>恋愛運</h3>
        <p>{{ love10}}</p>
        <h3>金銭運</h3>
        <p>{{ moeny10 }}</p>
        <h3>仕事運</h3>
        <p>{{ work10 }}</p>
      </div>
    </div>
    <div id="container" v-if='show'>
      <div id="con_left">
        <h1>{{ name11 }}</h1>
        <h2>総合運{{ point11 }}</h2>
        <p>{{ desciption11 }}</p>
        <table class="table">
          <tr>
            <th>今日のラッキーカラー</th>
            <td>{{ color11 }}</td>
          </tr>
          <tr>
            <th>今日のラッキーアイテム</th>
            <td>{{ item11 }}</td>
          </tr>
        </table>
      </div>
      <div id="con_right">
        <h3>恋愛運</h3>
        <p>{{ love11}}</p>
        <h3>金銭運</h3>
        <p>{{ moeny11 }}</p>
        <h3>仕事運</h3>
        <p>{{ work11 }}</p>
      </div>
    </div>
    <div id="container" v-if='show'>
      <div id="con_left">
        <h1>{{ name12 }}</h1>
        <h2>総合運{{ point12 }}</h2>
        <p>{{ desciption12 }}</p>
        <table class="table">
          <tr>
            <th>今日のラッキーカラー</th>
            <td>{{ color12 }}</td>
          </tr>
          <tr>
            <th>今日のラッキーアイテム</th>
            <td>{{ item12 }}</td>
          </tr>
        </table>
      </div>
      <div id="con_right">
        <h3>恋愛運</h3>
        <p>{{ love12}}</p>
        <h3>金銭運</h3>
        <p>{{ moeny12 }}</p>
        <h3>仕事運</h3>
        <p>{{ work12 }}</p>
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
  mounted() {
    // axios.get("/static/json/Aquarius.json").then((e) => {
    //   this.name = e.data.name;
    //   this.point = e.data.point;
    //   this.desciption = e.data.desciption;
    //   this.color = e.data.color;
    //   this.item = e.data.item;
    //   this.love = e.data.love;
    //   this.work = e.data.work;
    //   this.moeny = e.data.moeny;
    // }).catch((e) => {
    //   console.log("error")
    // });
    // axios.get("static/json/Aries.json").then((f) => {
    //   this.name2 = f.data.name;
    //   this.point2 = f.data.point;
    //   this.desciption2 = f.data.desciption;
    //   this.color2 = f.data.color;
    //   this.item2 = f.data.item;
    //   this.love2 = f.data.love;
    //   this.work2 = f.data.work;
    //   this.moeny2 = f.data.moeny;
    // });
    //  axios.get("static/json/Cancer.json").then((g) => {
    //   this.name3 = g.data.name;
    //   this.point3 = g.data.point;
    //   this.desciption3 = g.data.desciption;
    //   this.color3 = g.data.color;
    //   this.item3 = g.data.item;
    //   this.love3 = g.data.love;
    //   this.work3 = g.data.work;
    //   this.moeny3 = g.data.moeny;
    //  });
    //  axios.get("static/json/Capricorn.json").then((h) => {
    //   this.name4 = h.data.name;
    //   this.point4 = h.data.point;
    //   this.desciption4 = h.data.desciption;
    //   this.color4 = h.data.color;
    //   this.item4 = h.data.item;
    //   this.love4 = h.data.love;
    //   this.work4 = h.data.work;
    //   this.moeny4 = h.data.moeny;
    //  });
    //  axios.get("static/json/Gemini.json").then((i) => {
    //   this.name5 = i.data.name;
    //   this.point5 = i.data.point;
    //   this.desciption5 = i.data.desciption;
    //   this.color5 = i.data.color;
    //   this.item5 = i.data.item;
    //   this.love5 = i.data.love;
    //   this.work5 = i.data.work;
    //   this.moeny5 = i.data.moeny;
    // });
    //    axios.get("static/json/Leo.json").then((j) => {
    //   this.name6 = j.data.name;
    //   this.point6 = j.data.point;
    //   this.desciption6 = j.data.desciption;
    //   this.color6 = j.data.color;
    //   this.item6 = j.data.item;
    //   this.love6 = j.data.love;
    //   this.work6 = j.data.work;
    //   this.moeny6 = j.data.moeny;
    // });
    //   axios.get("static/json/Libra.json").then((k) => {
    //   this.name7 = k.data.name;
    //   this.point7 = k.data.point;
    //   this.desciption7 = k.data.desciption;
    //   this.color7 = k.data.color;
    //   this.item7 = k.data.item;
    //   this.love7 = k.data.love;
    //   this.work7 = k.data.work;
    //   this.moeny7 = k.data.moeny;
    // });
    //    axios.get("static/json/Pisces.json").then((m) => {
    //   this.name8 = m.data.name;
    //   this.point8 = m.data.point;
    //   this.desciption8 = m.data.desciption;
    //   this.color8 = m.data.color;
    //   this.item8 = m.data.item;
    //   this.love8 = m.data.love;
    //   this.work8 = m.data.work;
    //   this.moeny8 = m.data.moeny;
    // });
    //    axios.get("static/json/Sagittarius.json").then((n) => {
    //   this.name9 = n.data.name;
    //   this.point9 = n.data.point;
    //   this.desciption9 = n.data.desciption;
    //   this.color9 = n.data.color;
    //   this.item9 = n.data.item;
    //   this.love9 = n.data.love;
    //   this.work9 = n.data.work;
    //   this.moeny9 = n.data.moeny;
    // });
    //    axios.get("static/json/Scorpius.json").then((l) => {
    //   this.name10 = l.data.name;
    //   this.point10 = l.data.point;
    //   this.desciption10 = l.data.desciption;
    //   this.color10 = l.data.color;
    //   this.item10 = l.data.item;
    //   this.love10 = l.data.love;
    //   this.work10 = l.data.work;
    //   this.moeny10 = l.data.moeny;
    // });
    //     axios.get("static/json/Taurus.json").then((o) => {
    //   this.name11 = o.data.name;
    //   this.point11 = o.data.point;
    //   this.desciption11 = o.data.desciption;
    //   this.color11 = o.data.color;
    //   this.item11 = o.data.item;
    //   this.love11 = o.data.love;
    //   this.work11 = o.data.work;
    //   this.moeny11 = o.data.moeny;
    // });
    //    axios.get("static/json/Virgo.json").then((p) => {
    //   this.name12 = p.data.name;
    //   this.point12 = p.data.point;
    //   this.desciption12 = p.data.desciption;
    //   this.color12 = p.data.color;
    //   this.item12 = p.data.item;
    //   this.love12 = p.data.love;
    //   this.work12 = p.data.work;
    //   this.moeny12 = p.data.moeny;
    // });
  },
  data(){
    return {
      show: false,
      value1:'2018-07-20',
      name:'name',
      point:'point',
      desciption:'desciption',
      color:'color',
      item:'item',
      love:'love',
      work:'work',
      moeny:'moeny',
      name2:'name2',
      point2:'point2',
      desciption2:'desciption2',
      color2:'color2',
      item2:'item2',
      love2:'love2',
      work2:'work2',
      moeny2:'moeny2',
      name3:'name3',
      point3:'point3',
      desciption3:'desciption3',
      color3:'color3',
      item3:'item3',
      love3:'love3',
      work3:'work3',
      moeny3:'moeny3',
      name4:'name4',
      point4:'point4',
      desciption4:'desciption4',
      color4:'color4',
      item4:'item4',
      love4:'love4',
      work4:'work4',
      moeny4:'moeny4',
      name5:'name5',
      point5:'point5',
      desciption5:'desciption5',
      color5:'color5',
      item5:'item5',
      love5:'love5',
      work5:'work5',
      moeny5:'moeny5',
      name6:'name6',
      point6:'point6',
      desciption6:'desciption6',
      color6:'color6',
      item6:'item6',
      love6:'love6',
      work6:'work6',
      moeny6:'moeny6',
      name7:'name7',
      point7:'point7',
      desciption7:'desciption7',
      color7:'color7',
      item7:'item7',
      love7:'love7',
      work7:'work7',
      moeny7:'moeny7',
      name8:'name8',
      point8:'point8',
      desciption8:'desciption8',
      color8:'color8',
      item8:'item8',
      love8:'love8',
      work8:'work8',
      moeny8:'moeny8',
      name9:'name9',
      point9:'point9',
      desciption9:'desciption9',
      color9:'color9',
      item9:'item9',
      love9:'love9',
      work9:'work9',
      moeny9:'moeny9',
      name10:'name10',
      point10:'point10',
      desciption10:'desciption10',
      color10:'color10',
      item10:'item10',
      love10:'love10',
      work10:'work10',
      moeny10:'moeny10',
      name11:'name11',
      point11:'point11',
      desciption11:'desciption11',
      color11:'color11',
      item11:'item11',
      love11:'love11',
      work11:'work11',
      moeny11:'moeny11',
       name12:'name12',
      point12:'point12',
      desciption12:'desciption12',
      color12:'color12',
      item12:'item12',
      love12:'love12',
      work12:'work12',
      moeny12:'moeny12',
    }
  },
  methods:{
    Uranai:function(){
      if(this.value1 === '2018-07-20'){
      this.show = true;
      console.log(this.value1);
      console.log(this.data);
      axios.get("/static/json/Aquarius.json").then((e) => {
      this.name = e.data.name;
      this.point = e.data.point;
      this.desciption = e.data.desciption;
      this.color = e.data.color;
      this.item = e.data.item;
      this.love = e.data.love;
      this.work = e.data.work;
      this.moeny = e.data.moeny;
      // e.data.forEach(function(value,index,array){
      //   console.log(value);
      // });
    });
    axios.get("static/json/Aries.json").then((f) => {
      this.name2 = f.data.name;
      this.point2 = f.data.point;
      this.desciption2 = f.data.desciption;
      this.color2 = f.data.color;
      this.item2 = f.data.item;
      this.love2 = f.data.love;
      this.work2 = f.data.work;
      this.moeny2 = f.data.moeny;
    });
     axios.get("static/json/Cancer.json").then((g) => {
      this.name3 = g.data.name;
      this.point3 = g.data.point;
      this.desciption3 = g.data.desciption;
      this.color3 = g.data.color;
      this.item3 = g.data.item;
      this.love3 = g.data.love;
      this.work3 = g.data.work;
      this.moeny3 = g.data.moeny;
     });
     axios.get("static/json/Capricorn.json").then((h) => {
      this.name4 = h.data.name;
      this.point4 = h.data.point;
      this.desciption4 = h.data.desciption;
      this.color4 = h.data.color;
      this.item4 = h.data.item;
      this.love4 = h.data.love;
      this.work4 = h.data.work;
      this.moeny4 = h.data.moeny;
     });
     axios.get("static/json/Gemini.json").then((i) => {
      this.name5 = i.data.name;
      this.point5 = i.data.point;
      this.desciption5 = i.data.desciption;
      this.color5 = i.data.color;
      this.item5 = i.data.item;
      this.love5 = i.data.love;
      this.work5 = i.data.work;
      this.moeny5 = i.data.moeny;
    });
       axios.get("static/json/Leo.json").then((j) => {
      this.name6 = j.data.name;
      this.point6 = j.data.point;
      this.desciption6 = j.data.desciption;
      this.color6 = j.data.color;
      this.item6 = j.data.item;
      this.love6 = j.data.love;
      this.work6 = j.data.work;
      this.moeny6 = j.data.moeny;
    });
      axios.get("static/json/Libra.json").then((k) => {
      this.name7 = k.data.name;
      this.point7 = k.data.point;
      this.desciption7 = k.data.desciption;
      this.color7 = k.data.color;
      this.item7 = k.data.item;
      this.love7 = k.data.love;
      this.work7 = k.data.work;
      this.moeny7 = k.data.moeny;
    });
       axios.get("static/json/Pisces.json").then((m) => {
      this.name8 = m.data.name;
      this.point8 = m.data.point;
      this.desciption8 = m.data.desciption;
      this.color8 = m.data.color;
      this.item8 = m.data.item;
      this.love8 = m.data.love;
      this.work8 = m.data.work;
      this.moeny8 = m.data.moeny;
    });
       axios.get("static/json/Sagittarius.json").then((n) => {
      this.name9 = n.data.name;
      this.point9 = n.data.point;
      this.desciption9 = n.data.desciption;
      this.color9 = n.data.color;
      this.item9 = n.data.item;
      this.love9 = n.data.love;
      this.work9 = n.data.work;
      this.moeny9 = n.data.moeny;
    });
       axios.get("static/json/Scorpius.json").then((l) => {
      this.name10 = l.data.name;
      this.point10 = l.data.point;
      this.desciption10 = l.data.desciption;
      this.color10 = l.data.color;
      this.item10 = l.data.item;
      this.love10 = l.data.love;
      this.work10 = l.data.work;
      this.moeny10 = l.data.moeny;
    });
        axios.get("static/json/Taurus.json").then((o) => {
      this.name11 = o.data.name;
      this.point11 = o.data.point;
      this.desciption11 = o.data.desciption;
      this.color11 = o.data.color;
      this.item11 = o.data.item;
      this.love11 = o.data.love;
      this.work11 = o.data.work;
      this.moeny11 = o.data.moeny;
    });
       axios.get("static/json/Virgo.json").then((p) => {
      this.name12 = p.data.name;
      this.point12 = p.data.point;
      this.desciption12 = p.data.desciption;
      this.color12 = p.data.color;
      this.item12 = p.data.item;
      this.love12 = p.data.love;
      this.work12 = p.data.work;
      this.moeny12 = p.data.moeny;
    });

       }else if(this.value1 === '2018-06-19'){
        this.show = false;
        axios.get('static/json/20180619/Aquarius.json').then((q) => {
          console.log(q.data);
        })
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
