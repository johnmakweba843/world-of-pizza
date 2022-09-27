<template> 
  <header v-bind:class = "heading"> 
    <h2 v-bind:style = "{fontSize:size + 'px' , 
textAlign:align , fontWeight:weis , textTransform:trans ,  
fontStyle:sty }">{{name}}</h2>
  </header> 
  <main v-bind:class = "man"> 
    <h2 v-bind:class = "boss">{{toggle ()}}</h2> 
    <button v-bind:id = "nas" v-on:click = "paras = 'the world of niggasfood'">change now</button>
    <p v-bind:id = "butter" v-for = "resta in restas" :key = "resta">{{resta}}</p>  
    <h3 v-bind:id = "hoes">{{count}}</h3> 
    <button v-bind:class = "botch" v-on:click = "count += 1">count now</button>
</main>  

<form v-bind:class = "kiss" @submit.prevent = "submitForm"> 
 <input type = "text" id = "username" placeholder = "username" v-model.trim.lazy = "formValues.username" /> 
 <input type = "password" id = "password" placeholder="password" v-model.trim.lazy = "formValues.password" /> 
 <label v-bind:class = "dogs" for = "remoteWork">accept terms and conditions</label> 
 <input v-bind:class = "mouse" type="checkbox"  id="remoteWork" v-model = "formValues.remoteWork" true-value = "yes" false-value = "no" /> 
 <button v-bind:id = "rose" onclick = "alert('you are hacked')" v-on:click = "name = 'the world of burgers'">submit</button>
</form>   

</template> 

<script> 
 export default{ 
    data() {
        return{ 
            name:'the world of pizza',  
            size:18, 
            align:'center', 
            weis:800, 
            sty:'italic', 
            trans:'uppercase', 
            heading:'active', 
            paras:"the world of burgers", 
            man:'damn', 
            boss:'hero', 
            nas:'mama', 
            restas:['pizza' , 'amaranth' , 'burger'], 
            butter:'duck', 
            count:0, 
            hoes:'niggas', 
            botch:'box',  
            kiss:'search-box', 
            rose:'boco', 
            dogs:'cats', 
            mouse:'jerry',
            formValues:{ 
                username:'', 
                password:'', 
                remoteWork:"no"
            }
        }
    }, 
    methods:{ 
        toggle(){ 
            return this.paras
        }, 
        submitForm(){ 
            console.log("form Values" , this.formValues)
        }
    }
 }
</script> 

<style lang = "css"> 
 *{ 
    margin:0; 
    padding:0; 
    box-sizing:border-box; 
 } 

 .active{ 
    width:100%; 
    padding:10px 15px; 
    background-color:aquamarine; 
    box-shadow:2px 4px 4px rgba(200 , 10 , 0.5);
 } 

 .damn{ 
    display:flex; 
    align-items:center;  
    justify-content:center; 
    flex-direction:column;
 } 

 .hero{ 
    font-size:14px; 
    letter-spacing:1.2px; 
    font-weight:800;  
    margin-top:20px;
    text-transform:uppercase; 
    font-style:italic;
 } 

 #mama{ 
    width:100%; 
    max-width:200px; 
    background-color:rgb(255, 127, 229);
    color:#000; 
    font-size:18px;  
    margin-top:20px;
    margin-bottom:20px;
    font-weight:800; 
    font-style:italic; 
    cursor:pointer; 
    padding:10px 16px; 
    border-radius:1rem; 
    border:none; 
    text-transform:uppercase; 
    box-shadow:2px 8px 4px rgba(100 , 0 , 10); 
    transition:0.3s ease-in-out; 
 } 

 #mama:hover{ 
    color:#1a1a1a;  
    font-weight:800; 
    font-style:italic; 
    background:#fff; 
    border:3px solid orange;
 } 

 #duck{ 
    font-size:18px; 
    font-weight:800; 
    font-style:italic; 
    text-transform:capitalize; 
    letter-spacing:1.2px; 
    line-height:1.2rem; 
    padding-top:20px;
 } 

 #niggas{ 
    font-size:18px; 
    font-weight:800; 
    font-style:italic; 
    margin:10px 0;
 } 

 .box{ 
    width:100%; 
    max-width:200px; 
    background-color:rgb(214, 162, 39);
    color:#000; 
    font-size:18px;  
    margin-top:20px;
    margin-bottom:20px;
    font-weight:800; 
    font-style:italic; 
    cursor:pointer; 
    padding:10px 16px; 
    border-radius:1rem; 
    border:none; 
    text-transform:uppercase; 
    box-shadow:2px 8px 4px rgba(100 , 0 , 10); 
    transition:0.3s ease-in-out; 
 } 

 .box:hover{ 
    color:#000; 
    background:#fff; 
    border:3px solid orange;
 } 

 .search-box{ 
    display:flex; 
    align-items:center; 
    justify-content:center; 
    flex-direction:column;
 } 

 input{ 
    outline:none;
 } 

 input[type = "text"]{ 
    width:100%; 
    padding:10px 15px; 
    background:aquamarine; 
    color:#000; 
    font-size:18px; 
    font-weight:800; 
    margin-left:10px; 
    font-style:italic; 
    border-radius:8px; 
    border:none; 
 } 

 input[type = "text"]::placeholder{ 
    color:#000; 
    font-size:18px; 
    font-weight:800; 
    font-style:italic;
 }  



 input[type = "password"]{ 
    width:100%; 
    padding:10px 15px; 
    background:aquamarine; 
    color:#000; 
    font-size:18px;  
    margin-top:10px; 
    margin-bottom:15px;
    font-weight:800; 
    margin-left:10px; 
    font-style:italic; 
    border-radius:8px; 
    border:none; 
 } 

 input[type = "password"]::placeholder{ 
    color:#000; 
    font-size:18px; 
    font-weight:800; 
    font-style:italic;
 } 
 
 #boco{ 
    width:100%; 
    max-width:200px; 
    background-color:rgb(51, 135, 30);
    color:#000; 
    font-size:18px;  
    margin-top:20px;
    margin-bottom:20px;
    font-weight:800; 
    font-style:italic; 
    cursor:pointer; 
    padding:10px 16px; 
    border-radius:1rem; 
    border:none; 
    text-transform:uppercase; 
    box-shadow:2px 8px 4px rgba(100 , 0 , 10); 
    transition:0.3s ease-in-out; 
 } 

 #boco:hover{ 
    color:#000; 
    background:#fff; 
    border:3px solid orange;
 }
 
 .cats{ 
    font-size:18px; 
    font-weight:800; 
    font-style:italic; 
    text-transform:capitalize; 
    letter-spacing:1.2px;
 } 

 .jerry{ 
    width:auto; 
    height:auto;  
    border-radius:1px; 
    border:1px solid #000; 
    margin:10px 0;
 } 

</style>