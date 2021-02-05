<template>
  <div class="home container-fluid">
    <div class="row mainRow">
      <div class="col-md-8">
        <div class="row formula">
          <div class="col-md-8">
            <div class="row">
            <div class="col-sm-6">Cost of Goods <input type="number" class="inputBox"></div>
            <div class="col-sm-6">Margin <input type="number" class="inputBox"> </div>
            
           
             </div>
             </div>
          <div class="col-md-3">| Sale Price</div>
        </div>
        <div class="row formula">
          <div class="col-md-8">Cost of Goods | Sale Price</div>
          <div class="col-md-3">| Margin</div>
        </div>
        <div class="row formula">
          <div class="col-md-8">Cost of Goods | Markup</div>
          <div class="col-md-3">| Sale Price</div>
        </div>
        <div class="row formula">
          <div class="col-md-8">Cost of Goods | Sale Price</div>
          <div class="col-md-3">| Markup</div>
        </div>
      </div>
      <div class="col-md-3 box">Examples</div>
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

.container-fluid {
  background-color: rgb(175, 29, 29);
}

.row {
  background-color: white;
}

.box {
  border: 1px solid rgb(158, 158, 158);
  margin: 10px;
}

.mainRow {
  margin-top: 50px;
}

.formula {
    border: 1px solid rgb(158, 158, 158);
  margin: 10px;
}

.inputBox {
  width: 80px;
}
</style>
