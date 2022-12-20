<template>
  <div class="cardHolder-container">
    <div class="cardHolder-wrap">
      <div class="cardHolder">
        <div class="cardHolder-nameTag">
          <b-row>
            <b-col cols="9" class="cardHolder-titleTag"
              >John Hardy Women's Legends Naga Gold & Silver Dragon Station Chain Bracelet</b-col
            >
          </b-row>
        </div>
        <!-- product goes here -->
        <img src="https://fakestoreapi.com/img/71pWzhdJNwL._AC_UL640_QL65_ML3_.jpg" />

        <!-- button I HAVE TO MAKE THIS AS A COMPONENT -->
        <div class="cardHolder-buttonsContainer">
          <button class="button-49" role="button">BUY NOW</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.cardHolder-container {
  margin-bottom: 300px;
  margin-left: 300px;
  margin-top: 100px;
}

.cardHolder-wrap {
  filter: drop-shadow(3px 6px 9px #cdcdcd80);

}
.cardHolder {
  /* background-color: #f4f4f4; */
  background-color: white;

  clip-path: polygon(0% 0%, 100% 0%, 100% 100%, 8% 100%, 0% 95%);
  border-right: 5px solid #30303080;
  min-width: 400px;
  min-height: 600px;
  max-width: 400px;
  min-height: 600px;
}

.cardHolder-titleTag {
  padding-left: 50px;
  background-color: #f2f2f232;
  border-radius: 500px;
  color: #222;
  font: bold 24px system-ui;
  z-index: 2;
  margin: 1rem;

}

.cardHolder-nameTag {
  min-width: 400px;

  max-width: 400px;
}

img {
  height:  300px;
  max-width: 300px;
  margin-left: 3rem;
  margin-top: 1rem;
  object-fit: contain;
}

/* Button style */
.cardHolder-buttonsContainer{
margin-top: 3rem;
margin-left: 5.5rem;
}
.button-49,
.button-49:after {
  width: 200px;
  height: 76px;
  line-height: 78px;
  font-size: 20px;
  font-family: "Bebas Neue", sans-serif;
  background: linear-gradient(45deg, transparent 5%, #363636 5%);
  border: 0;
  color: #fff;
  letter-spacing: 3px;
  box-shadow: 6px 0px 0px #616161;
  outline: transparent;
  position: relative;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
}

.button-49:after {
  --slice-0: inset(50% 50% 50% 50%);
  --slice-1: inset(80% -6px 0 0);
  --slice-2: inset(50% -6px 30% 0);
  --slice-3: inset(10% -6px 85% 0);
  --slice-4: inset(40% -6px 43% 0);
  --slice-5: inset(80% -6px 5% 0);

  content: "BUY NOW";
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(
    45deg,
    transparent 3%,

    #ababab 3%,

    #acacac 5%,
    /* background  */
    #080808 5%
  );
  text-shadow: -3px -3px 0px #f7f7f7;
  clip-path: var(--slice-0);
}

.button-49:hover:after {
  animation: 1s glitch infinite;
  animation-timing-function: steps(2, end);
}

@keyframes glitch {
  0% {
    clip-path: var(--slice-1);
    transform: translate(-20px, -10px);
  }
  10% {
    clip-path: var(--slice-3);
    transform: translate(10px, 10px);
  }
  20% {
    clip-path: var(--slice-1);
    transform: translate(-10px, 10px);
  }
  30% {
    clip-path: var(--slice-3);
    transform: translate(0px, 5px);
  }
  40% {
    clip-path: var(--slice-2);
    transform: translate(-5px, 0px);
  }
  50% {
    clip-path: var(--slice-3);
    transform: translate(5px, 0px);
  }
  60% {
    clip-path: var(--slice-4);
    transform: translate(5px, 10px);
  }
  70% {
    clip-path: var(--slice-2);
    transform: translate(-10px, 10px);
  }
  80% {
    clip-path: var(--slice-5);
    transform: translate(20px, -10px);
  }
  90% {
    clip-path: var(--slice-1);
    transform: translate(-10px, 0px);
  }
  100% {
    clip-path: var(--slice-1);
    transform: translate(0);
  }
}
</style>