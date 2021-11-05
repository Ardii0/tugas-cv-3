<template>
<div class="bord">
    <div class="kiri">
        <div style="display: flex;">
            <div class="1">
            <h1 v-for="user in users" :key="user" 
            class="tex">{{ user.frs }} <br><span class="nama">{{ user.sc }}</span><span class="nama2">{{ user.trd }}</span></h1><br>
              <img src="https://asset-a.grid.id/crop/0x0:0x0/x/photo/2018/09/12/1506637489.jpg">
            <h2 class="tex">Contact<hr class="line"></h2>
            <p class="tex">
                <strong>Address:</strong><br>
            </p>
            <p v-for="user in users" :key="user" class="tex"> 
                {{ user.alamat }}
            </p>
                <strong class="tex">Phone:</strong>
            <p v-for="user in users" :key="user" class="tex">
                {{ user.phone}} 
            </p>
            <strong class="tex">Email:</strong>
            <p v-for="user in users" :key="user" class="tex">
            {{ user.email }} 
            </p>
            <h2 class="tex">Languages<hr class="line"></h2>
                <p v-for="user in users" :key="user" class="tex">
                    {{ user.bahasa1 }}</p> 
                <p v-for="user in users" :key="user" class="tex">
                    {{ user.bahasa2 }}</p> 
            <h2 class="tex">Hobbies<hr class="line"></h2>
                <ul v-for="user in users" :key="user" 
             class="tex2">
                    <li>{{ user.hob}}</li>
                    <li>{{ user.hobi}}</li>
                </ul>
            </div>
        <div class="kanan">
             <h2 class="kata">Summary<hr class="line">
            </h2>
            <p class="kata" v-for="user in users" :key="user">
                {{ user.ringkasan }}
            </p>
               <h2 class="kata">Skill Highlights<hr class="line">
               </h2>
               <ul class="tex2">
                   <li v-for="user in users" :key="user" 
               >{{ user.sh }}</li>
                   <li v-for="user in users" :key="user" 
               >{{ user.sh2 }}</li>
               </ul>
               <br>
               <h2 class="kata">Experience<hr class="line">
               </h2>
               <p v-for="user in users" :key="user" 
               class="kata"><strong>{{ user.exno }}</strong><span>{{ user.exto }}</span></p>
               <ul class="tex2">
                   <li><strong>Didn't join any Project yet...</strong></li>
               </ul>
               <br>
               <h2 class="kata">Education<hr class="line">
               </h2>
               <p class="kata">SMK :<strong v-for="user in users" :key="user">{{ user.smk }}</strong> - 2021</p>
               <br>
               <h2 class="kata">Certifications<hr class="line">
               </h2>
               <p class="kata">Programming : 
                   <strong v-for="user in users" :key="user">
                    {{ user.prog }}</strong></p> 
    </div>
    </div>
</div>
</div>
</template>

<script>
/* eslint-disable */
import axios from 'axios'
export default {
    name : "CvSatu",
data(){
  return{
    users: '',
  }
},
  mounted() {
    this.load()
  },
  methods: {
    load(){
      axios.get('http://localhost:3000/users').then(res => {
      this.users = res.data
      }).catch ((err) => {
        console.log(err);
      })
    }
  }
  }
</script>
<style>
.bord {
    background-color: gray;
    padding-top: 50px;
    padding-bottom: 50px;
}
.kiri {
    margin-left: 300px;
    height: 940px;
    width: 750px;
    border: none;
    background-color: silver;
    padding-bottom: 20px;
    font-family: sans-serif;
}
img {
    height: 200px;
    width: 300px;
}
.kanan {
    height: 960px;
    width: 450px;
    border: none;
    background-color: white;
    text-align: left;
}
.nama {
    color: coral;
}   
.nama2 {
    color: aliceblue;
}
.line {
    height: 2px;
    background-color:  darkgray;
}
.kata {
    padding-left: 20px;
    padding-right: 20px;
}
.tex {
    padding-left: 20px;
    padding-right: 10px;
}
.tex2 {
    padding-left: 100px;
    padding-right: 10px;
}
</style>