<script lang="ts">
  let A=0
  let B=0
  let C=0
  let D=0
  let E=0
  let F=0
  let G=0
  let H=0
</script>

<main>
<div class="root">
  <div class="title">2023年度物理学院 自强大学生标兵 答辩唱票</div>
  <div class="row">
    <div class="element">
      <button class="button" on:click={()=>{A+=1}}>{A}</button>
      <div class="child">李弘禹</div>
    </div>
    <div class="element">
      <button class="button" on:click={()=>{B+=1}}>{B}</button>
      <div class="child">葛景业</div>
    </div>
    <div class="element">
      <button class="button" on:click={()=>{C+=1}}>{C}</button>
      <div class="child">谯宇箫</div>
    </div>
    <div class="element">
      <button class="button" on:click={()=>{D+=1}}>{D}</button>
      <div class="child">邱卓伦</div>
    </div>
  </div>
  <div class="row">
    <div class="element">
      <button class="button" on:click={()=>{E+=1}}>{E}</button>
      <div class="child">刘嘉新</div>
    </div>
    <div class="element">
      <button class="button" on:click={()=>{F+=1}}>{F}</button>
      <div class="child">肖守宇</div>
    </div>
    <div class="element">
      <button class="button" on:click={()=>{G+=1}}>{G}</button>
      <div class="child">马喆</div>
    </div>
    <div class="element">
      <button class="button" on:click={()=>{H+=1}}>{H}</button>
      <div class="child">杨炅然</div>
    </div>
  </div>

</div >
</main>

<style>
  .root{
    margin-left: 5vw;
    width: 90vw;
    height: 100vh;
    display: flex;
    flex-direction: column;

  }
  .element{
    width: 90%;
    margin-left: 5%;
    margin-right: 5%;
    height: 95%;
    margin-bottom: 5%;
  }
  .child{
    height: 40%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 50px;
    font-weight: bold;
  }
  .title{
    width: 100%;
    height: 20%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 60px;
    font-weight: bold;
  }
  .row{
    width: 100%;
    height: 40%;
    display: flex;
    flex-direction: row;
  }
  .button {
    position: relative;
    background-color: #0086fc;
    border: none;
    font-size: 100px;
    font-weight: bolder;
    color: #FFFFFF;
    padding: 20px;
    width: 100%;
    height: 60%;
    border-radius: 10px;
    text-align: center;
    -webkit-transition-duration: 0.4s; /* Safari */
    transition-duration: 0.4s;
    text-decoration: none;
    overflow: hidden;
    cursor: pointer;
  }

  .button:after {
    content: "";
    background: #47a8ff;
    display: block;
    position: absolute;
    padding-top: 300%;
    padding-left: 350%;
    margin-left: -20px!important;
    margin-top: -120%;
    opacity: 0;
    transition: all 0.8s
  }

  .button:active:after {
    padding: 0;
    margin: 0;
    opacity: 1;
    transition: 0s
  }
</style>
