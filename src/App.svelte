<script>
  import Navbar from './lib/Navbar.svelte'
  import CTA from './lib/CTA.svelte'
  function cardClick() {
        document.querySelector('.card').style.display='none';
    }

    function adPop() {
      document.querySelector('.popup').style.display='flex';
    }


</script>

<main>
  <Navbar />
  <div class="container">
  <h1 on:mouseover={adPop}>Make Simple <br> with One <a class="red">Card</a></h1>
  <CTA />


  <p>CARD is the digital payment services. With one card you can<br> manage your daily financial and also can <a class="red">get more benefits</a></p>
  <img on:click={cardClick} src="https://pngimg.com/d/credit_card_PNG204.png" class="card" alt="card">
  <img on:click={cardClick} src="https://pngimg.com/d/credit_card_PNG204.png" class="card" alt="card">
  <img on:click={cardClick} src="https://pngimg.com/d/credit_card_PNG204.png" class="card" alt="card">
</div>

</main>

<style>

.container {
  margin: 10vh;
}
  h1 {
    font-size: 48px;
    line-height: 48px;
  }

  .red {
    color: red;
  }
.card {
  height: 20vh;
  margin: 16px;
}

.card:hover {
  scale: 1.04;
  transform: translateY(-1vh);
  cursor: pointer;
  transition: 400ms;
}

p {
  text-align: right;
}

p .red {
  cursor: pointer;
}

.card:nth-child(2) {
  padding: 0px;
}


</style>