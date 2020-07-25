<template>
  <div class="page">
    <div class="page_scroll">
      <div class="card card--long card--dawn"></div>
      <div class="card card--daylight"></div>
      <div class="card card--long card--daylight-sunset"></div>
      <div class="card card--small card-sunset-orange"></div>
      <div class="card card--long card--sunset"></div>
      <div class="card card--night"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.page {
  display: flex;
  overflow: hidden;

  flex-direction: column;
  justify-content: center;
  align-items: center;

  height: 100vh;
  padding: 2rem;
}

.page_scroll {
  overflow: scroll;

  flex: 1;

  width: 100%;
  height: 100%;

  background: black;
}

.card {
  position: relative;

  display: flex;
  overflow: hidden;

  align-items: flex-end;

  width: 100%;
  height: 100vh;
}

.card--long {
  height: 200vw;
}

.card--small {
  height: 25vw;
}

.card--night {
  background-image: linear-gradient(
    0deg,
    hsl(0, 0%, 0%) 0%,
    hsla(0, 0%, 0%, 0.738) 19%,
    hsla(0, 0%, 0%, 0.541) 34%,
    hsla(0, 0%, 0%, 0.382) 47%,
    hsla(0, 0%, 0%, 0.278) 56.5%,
    hsla(0, 0%, 0%, 0.194) 65%,
    hsla(0, 0%, 0%, 0.126) 73%,
    hsla(0, 0%, 0%, 0.075) 80.2%,
    hsla(0, 0%, 0%, 0.042) 86.1%,
    hsla(0, 0%, 0%, 0.021) 91%,
    hsla(0, 0%, 0%, 0.008) 95.2%,
    hsla(0, 0%, 0%, 0.002) 98.2%,
    hsla(0, 0%, 0%, 0) 100%
  );
  background-color: #161836;
}

.card--sunset {
  background: linear-gradient(0deg, #161836 0%, #382e4b 20%, #f98056 60%);
}

.card-sunset-orange {
  background-color: #e9e28b;

  background-image: linear-gradient(
    0deg,
    hsl(15, 93%, 66%) 0%,
    hsl(15, 93%, 66%, 0.738) 19%,
    hsl(15, 93%, 66%, 0.541) 34%,
    hsl(15, 93%, 66%, 0.382) 47%,
    hsl(15, 93%, 66%, 0.278) 56.5%,
    hsl(15, 93%, 66%, 0.194) 65%,
    hsl(15, 93%, 66%, 0.126) 73%,
    hsl(15, 93%, 66%, 0.075) 80.2%,
    hsl(15, 93%, 66%, 0.042) 86.1%,
    hsl(15, 93%, 66%, 0.021) 91%,
    hsl(15, 93%, 66%, 0.008) 95.2%,
    hsl(15, 93%, 66%, 0.002) 98.2%,
    hsl(15, 93%, 66%, 0) 100%
  );
}

.card--daylight-sunset {
  background: linear-gradient(
    180deg,
    #5c7cc2 0%,
    #5c7cc2 19%,
    #6a86bc 34%,
    #7891b7 47%,
    #869bb1 56.5%,
    #94a5ac 65%,
    #a2afa7 73%,
    #b1b9a1 80.2%,
    #bfc39c 86.1%,
    #cdce96 91%,
    #dbd891 95.2%,
    #e9e28b 98.2%,
    #e9e28b 100%
  );
}

.card--daylight {
  background: linear-gradient(
    0deg,
    #5c7cc2 0%,
    #6d9ed7 34%,
    #6bafd2 67%,
    #a4c8dc 100%
  );
}
.card--dawn {
  background: linear-gradient(
    0deg,
    #a4c8dc 0%,
    #b4d9e1 38%,
    #d6cbca 58%,
    #eabc96 79%,
    #db8876 100%
  );
}
</style>
