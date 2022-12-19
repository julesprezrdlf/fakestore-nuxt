<template>
  <div class="cardHolder-container">
    <div class="cardHolder-wrap">
      <div class="cardHolder">
        <div class="cardHolder-nameTag">
          <b-row>
            <b-col cols="8" class="cardHolder-titleTag"
              >Mens Cotton Jacket</b-col
            >
          </b-row>
        </div>
        <!-- product goes here -->
        <img src="https://fakestoreapi.com/img/71li-ujtlUL._AC_UX679_.jpg"/>
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
  filter: drop-shadow(3px 6px 9px rgba(205, 205, 205, 0.5));
}
.cardHolder {
  /* background-color: #f4f4f4; */
  background-color: white;

  clip-path: polygon(100% 0%, 100% 90%, 85% 100%, 0% 100%, 0% 0%);

  min-width: 400px;
  min-height: 700px;
  max-width: 400px;
  min-height: 700px;
}

.cardHolder-titleTag {
  padding-left: 50px;
  background-color: #f2f2f232;
  border-radius: 500px;
  color: #222;
  font: bold 32px system-ui;
  z-index: 2;
  margin: 1rem;


}

.cardHolder-nameTag {
  min-width: 400px;

  max-width: 400px;
}

img{
    width: 300px;
margin-left: 3rem;
margin-top: 1rem;
}
</style>