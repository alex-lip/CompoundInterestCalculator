<template>
  <div class="home container-sm">
        <div class="row formula">
              <div class="col-sm-4 box1">
                Cost of Goods <input type="number" class="inputBox" />
              </div>
              <div class="col-sm-3 box2">
                Margin <input type="number" class="inputBox" />
              </div>
              <div class="col-sm-4 box3">Sale Price</div>
            </div>
          </div>
</template>

<script>
export default {
  name: "home",
};
</script>

<style scoped>
input::-webkit-outer-spin-button,
input::-webkit-inner-spin-button {
  -webkit-appearance: none;
  margin: 0;
}

.mainRow {
  margin-top: 50px;
}

.formula {
  border: 1px solid rgb(223, 223, 223);
  padding: 15px 2px;
  font-size: 22px;
  background-color: white;
}

.inputBox {
  width: 80px;
}
/*
.box1 {
  background-color: red;
}

.box2 {
  background-color: blue;
}

.box3 {
  background-color: green;
}

*/
</style>
