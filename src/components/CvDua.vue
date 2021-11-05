<template>
    <div class="all">
        <div class="bg"></div>
    <div class="res">RESUME</div>
    <div class="jud">
      <div class="gb">
        <img class="gm" src="https://www.pngitem.com/pimgs/m/504-5040528_empty-profile-picture-png-transparent-png.png">
      </div>
        <div class="name">
            <h1>MUHAMMAD <br> ARDI<span class="lastn">SETIAWAN</span></h1>
        </div>
        <div class="kotak">
           <h1>PROGRAMMER<hr class="lm"></h1> 
        <div class="right">
        <p class="title"><i style="font-size: 30px" class="fas fa-briefcase"></i>
        <span style="padding-left: 5px">
          WORK EXPREIENCE</span> <hr class="dashed2">
            <div class="kurung">
        <div style="display: flex; margin-left: 20px; margin-right: 20px;">
                      <p v-for="user in bio" :key="user">
                        {{ user.none }}</p>
                </div>
        </div>
        </div>
        <br>
        <div class="right2">
        <p class="title"><i style="font-size: 30px" class="fas fa-book"></i><span style="padding-left: 5px">
          EDUCATION</span><hr class="dashed2">
            <div class="kurung">
                <div style="margin-left: 20px; margin-right: 20px;">
                        <p v-for="user in bio" :key="user"><b>{{ user.sd }}</b></p>
                        <p v-for="user in bio" :key="user">
                        {{ user.sch }}</p><br>
                        <p v-for="user in bio" :key="user"><b>{{ user.smp }}</b></p>
                        <p v-for="user in bio" :key="user">
                        {{ user.smid }}</p><br>
                        <p v-for="user in bio" :key="user"><b>{{ user.smk}}</b></p>
                        <p v-for="user in bio" :key="user">
                        {{ user.sekul }}</p>
                </div>
            </div>
        </div>
        <br>
        <div class="right3">
          <div class="kurung">
              <div class="ges">
              <h4 class="h">PERSONAL SKILLS</h4>
              <p>Organisation<span style="margin-left: 31px">&#9899;&#9899;&#9899;&#9899;</span><span style="opacity: 0.5">&#9899;&#9899;</span></p>
              <p>Communication<span style="margin-left: 9px;">&#9899;&#9899;&#9899;&#9899;</span><span style="opacity: 0.5">&#9899;&#9899;</span></p>
              <p>Time Keeping<span style="margin-left: 23px">&#9899;&#9899;&#9899;&#9899;</span><span style="opacity: 0.5">&#9899;&#9899;</span></p>
              <p>Team Player<span style="margin-left: 33px">&#9899;&#9899;&#9899;&#9899;</span><span style="opacity: 0.5">&#9899;&#9899;</span></p>
              <p>Commitment<span style="margin-left: 31px">&#9899;&#9899;&#9899;&#9899;</span><span style="opacity: 0.5">&#9899;&#9899;</span></p>
              <p>Multitasking<span style="margin-left: 37px">&#9899;&#9899;&#9899;&#9899;</span><span style="opacity: 0.5">&#9899;&#9899;</span></p>
              </div>
              </div>
        <p class="title"><i style="font-size: 30px" class="fas fa-lightbulb"></i><span style="padding-left: 5px">
          SKILLS</span><hr class="dashed2">
            <div class="kurung">
              <h4 class="h">PROFESSIONAL SKILLS</h4>
              <p>Microsoft Windows<span style="margin-left:5px">&#9899;&#9899;&#9899;&#9899;</span><span style="opacity: 0.5">&#9899;&#9899;</span></p>
              <p>Windows<span style="margin-left: 74px">&#9899;&#9899;&#9899;&#9899;</span><span style="opacity: 0.5">&#9899;&#9899;</span></p>
              <p>Mac OSX<span style="margin-left: 70px">&#9899;&#9899;&#9899;&#9899;</span><span style="opacity: 0.5">&#9899;&#9899;</span></p>
              <p>Data Handling<span style="margin-left: 37px">&#9899;&#9899;&#9899;&#9899;</span><span style="opacity: 0.5">&#9899;&#9899;</span></p>
              <p>Record Keeping<span style="margin-left: 25px">&#9899;&#9899;&#9899;&#9899;</span><span style="opacity: 0.5">&#9899;&#9899;</span></p>
              <p>Web Skills<span style="margin-left: 65px">&#9899;&#9899;&#9899;&#9899;</span><span style="opacity: 0.5">&#9899;&#9899;</span></p>
            </div>
        </div>
    </div>
    </div>
    <div class="prof">
        <p class="title">PROFILE<hr class="dashed">
        <div class="kurung">
            <h3 class="h">NAME</h3>
        <p class="h" v-for="user in bio" :key="user">
            {{ user.nama }}</p>
            <h3 class="h">DATE OF BIRTH</h3>
        <p class="h" v-for="user in bio" :key="user">
            {{ user.ultah }}</p>
            <h3 class="h">ADDRESS</h3>
        <p class="h" v-for="user in bio" :key="user">
        {{ user.addr }}</p>
        <p class="h" v-for="user in bio" :key="user">
        {{ user.alam }}</p> 
        <p class="h" v-for="user in bio" :key="user">
        {{ user.mat }}</p>
            <h3 class="h">WEBSITE</h3>
        <p class="h" v-for="user in bio" :key="user">
            {{ user.web }}</p>
        </div>
        <p class="title">AWARDS<hr class="dashed">
        <p class="h" v-for="user in bio" :key="user">
          {{ user.none }}
        </p>
        <div class="kurung"></div>
        <p class="title">CONTACT<hr class="dashed">
        <div class="kurung">
            <span style='font-size:50px; position: absolute;'>&#9742;</span>
            <h3 class="h">HOME NUMBER</h3>
        <p class="h" v-for="user in bio" :key="user">{{ user.tw }}</p>
        <i style="font-size: 50px; position: absolute; margin-top: 10px" class="fas fa-phone-square-alt"></i>
            <h3 style="margin-right: 10px"
            class="h">PHONE NUMBER</h3>
        <p class="h" v-for="user in bio" :key="user" style="margin-right: 10px">
          {{ user.sphone }}</p><br>
        <i style="font-size: 50px; position: absolute; margin-top: 23px" class="fas fa-envelope-square"></i>
            <h3 style="margin-right: 10px" 
            class="h">EMAIL</h3>
        <p class="h" v-for="user in bio" :key="user" style="margin-right: 10px">
            {{ user.ehmail }}</p>
            </div><br>
        <p class="title">SOCIAL<hr class="dashed">
        <div class="kurung">
        <i style="font-size: 50px; position: absolute; margin-top: 5px" class="fab fa-tumblr-square"></i>
            <h3 style="margin-right: 10px"
            class="h">TWITTER</h3>
        <p v-for="user in bio" :key="user" style="margin-right: 10px">
          {{ user.tw }}</p>
        <i style="font-size: 50px; position: absolute; margin-top: 23px;" class="fab fa-facebook-square"></i>
            <h3 style="margin-right: 10px" 
            class="h">FACEBOOK</h3>
        <p v-for="user in bio" :key="user" style="margin-right: 10px">
            {{ user.fb }}</p>
            </div>
    </div>
    <div class="lastencore"></div>
    </div>
</template>

<script>
/* eslint-disable */
import axios from 'axios'
export default {
    name: "CvDua",
data(){
  return{
    bio: '',
  }
},
  mounted() {
    this.load()
  },
  methods: {
    load(){
      axios.get('http://localhost:3000/bio').then(res => {
      this.bio = res.data
      }).catch ((err) => {
        console.log(err);
      })
    }
  }
  }
</script>

<style>
.all {
    height: 960px;
    padding-bottom: 20px;
    font-family: 'Courier New', Courier, monospace;
}
      .bg {
        background-color: darkslateblue;
        height: 40px;
        margin-left: 100px;
        margin-right: 100px;
      }
      .res {
        background-color: darkslateblue;
        height: 1px;
        margin-left: 200px;
        width: 130px;
        color: white;
        font-size: 30px;
        text-align: center;
        padding-bottom: 40px;
      }
      .jud {
        background-color: darkslateblue;
        height: 150px;
        color: white;
        display: flex;
        margin-left: 100px;
        margin-right: 100px;
      }
      .gb {
        padding-top: 30px;
        margin-left: 100px;
      }
      .gm {
        width: 200px;
        height: 200px;
        display: flex;
        border-radius: 50%;
        margin-left: 20px;
        margin-left: 0px;
      }
      .name {
          padding-top: 20px;
          padding-left: 20px;
      }
      .lastn {
          padding-left: 7px;
      }
.prof {
    height: 760px;
    width: 350px;
    margin-top: 100px;
    border: none;
    background-color: white;
    text-align: right;
    padding-left: 50px;
    margin-left: 100px;
    padding-right: 20px;
}
     .dashed {
         border: dashed 1px black;
         width: 244px;
         margin-left: 120px;
     }
     .dashed2 {
         border: dashed 1px black;
     }
     .h {
         color: gray;
     }
     .kurung {
      font-family: sans-serif;
      padding-right: 10px;
     }
     .kotak {
         color: black;
         padding-top: 200px;
     }
     .lm {
         border: 1px solid black;
         width: 14cm;
         padding-left: 15px;
         padding-right: 25px;
     }
.right {
    height: 250px;
    width: 525px;
    border: none;
    background-color: silver;
    padding: 25px;
    padding-top: 5px;
    font-family: 'Courier New', Courier, monospace;
}
    .p {
        display: flex;
    }
.right2 {
    height: 400px;
    width: 525px;
    border: none;
    background-color: silver;
    padding: 25px;
    padding-top: 5px;
    font-family: 'Courier New', Courier, monospace;
}
.right3 {
    height: 355px;
    width: 525px;
    border: none;
    background-color: silver;
    padding: 25px;
    padding-top: 5px;
    font-family: 'Courier New', Courier, monospace;
}
.title {
    font-family: 'Courier New', Courier, monospace;
    font-size: 25px;
}
 .lastencore {
    background-color: darkslateblue;
    height: 40px;
    margin-top: 430px;
    margin-left: 100px;
    margin-right: 100px;
 }  
 .ges {
   position: absolute;
   margin-left: 270px;
   padding-top: 86px
 }
</style>