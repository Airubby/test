<template>
  <div id="gamecontainer">
    <canvas id="gamecanvas" width="640" height="480" class="gamelayer"></canvas>
    <div id="scorescreen" class="gamelayer">
      <img id="togglemusic" src="images/gameOne/icons/sound.png">
      <img src="images/gameOne/icons/prev.png">
      <span id="score">Score: 0</span>
    </div>
    
    <div id="gamestartscreen" class="gamelayer">
      <img src="images/gameOne/icons/play.png" alt="Play Game" onclick = "game.showLevelScreen();"><br>
      <img src="images/gameOne/icons/settings.png" alt="Settings">
    </div>
    
    <div id="levelselectscreen" class="gamelayer">
    </div>
    
    <div id="loadingscreen" class="gamelayer">
      <div id="loadingmessage"></div>
    </div>
    
    <div id="endingscreen" class="gamelayer">
      <div>
        <p id="endingmessage">The Level Is Over Message</p>
        <p id="playcurrentlevel"><img src="images/gameOne/icons/prev.png"> Replay Current Level</p>				
        <p id="playnextlevel"><img src="images/gameOne/icons/next.png"> Play Next Level </p>				
        <p id="showLevelScreen"><img src="images/gameOne/icons/return.png"> Return to Level Screen</p>
      </div>
    </div>	
  </div>
</template>

<script>

export default {
  name: 'home',
  created () {
  },
  mounted() {
    game.init();
  },
  data() {
      return {

      }
  },
  methods:{
      
  },
  components:{}
}
</script>
<style scoped lang="less">
  
</style>
