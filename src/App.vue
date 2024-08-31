<template>
  <div class="name">{{ name }}</div>
  <h1>여기 좋다 ☺️</h1>
  <h3>집에서 뭐하나 했더니.... 놀게 디게 많네....</h3>

  <div class="contents"> 
    <div class="sanga">
      <button @click="showAlert">히히히</button>
    </div>
    <div class="pul">
      해헤헤
    </div>
  </div>
</template>

<script>
// 왜 setup으로 알려주지.....
export default {
  setup() {
    const name = 'Es ist ziemlich lustig';
    const showAlert = () => {
      console.log("메롱")
    }

    return {
      name,
      showAlert
    }
  }
}
</script>

<style>
  .name {
    color: blue;
    font-size: 100px;
    font-weight: 900;
  }

  .contents {
    display: flex;
    background-color: green;
  }

  .sanga {
    width: 50%;
    height: 30vh;
    background-color: red;
  }

  .pul {
    width: 50%;
  }


</style>