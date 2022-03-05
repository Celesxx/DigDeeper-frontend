<template>

  <div class="home-body">

    <div class="body-presentation">

      <div class="presentation-description">

        <h1 id="description-title">Mine more to get more</h1>

        <p id="description-text">
          DigDeeper is an on-chain idle game based on the rewards. 
          The goal is simple, mine more and craft you'r best strategy to find and get more gems.
        </p>

      </div>

      <div class="presentation-core">

        <div class="core-description" id="core-competence">
          <img alt="skill" id="skill-logo" src="../../assets/skills.png"> 
          <p id="skill-text">Get a miner and start the adventure </p>
        </div>

        <div class="core-description" id="core-tool">
          <img alt="setting" id="setting-logo" src="../../assets/settings.png"> 
          <p id="skill-text">upgrade your mining skill to be the best miner and get more</p>
        </div>

        <div class="core-description" id="core-withdraw">
          <img alt="reward" id="reward-logo" src="../../assets/reward.png"> 
          <p id="skill-text">upgrade your mining skill to be the best miner and get more</p>
        </div>

      </div>

    </div>





    <div class="body-rule">

      <div class="rule-global">

        <div class="rule-description">

          <h1 id="rule-title">Buy miner</h1>
          <p id="rule-text">
            To start the adventure and find so many gems you need to buy one or many miner 
          </p>

          <input type="text" id="form-input" name="form-buy">
          <p id="rule-terms">
            Miners are utility NFTs solely intended for to our DigDeeper game 
            that carry no expectation of profit and have no guaranteed resale value. 
            By buying you agree to the Terms of Service.
          </p>

          <button id="form-button" type="button" name="metaMask">
              install Metamask  
          </button>

        </div> 

        
      </div>

      <div class="rule-game">
          
      </div>
    </div>

  </div>
</template>

<script>
export default 
{
  name: 'HomeComponent'
}
</script>

<style scoped>
    @import '../../assets/styles/global/web/home.css';
    @import '../../assets/styles/global/mobile/home.css';
</style>
