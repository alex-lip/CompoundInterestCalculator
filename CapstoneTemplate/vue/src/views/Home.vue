<template>
  <div class="home container-sm">
    <div class="row formula">
      <div class="col-sm-4">
        Cost of Goods <input type="number" class="inputBox" v-model="cogs1" />
      </div>
      <div class="col-sm-3">
        Margin <input type="number" class="inputBox" v-model="margin" /> %
      </div>
      <div class="col-sm-4">Sale Price: {{ cogsMargin }}</div>
    </div>


    <div class="row formula">
      <div class="col-sm-4">
        Cost of Goods <input type="number" class="inputBox" v-model="cogs2" />
      </div>
      <div class="col-sm-3">
        Sale Price <input type="number" class="inputBox" v-model="salePrice1" />
      </div>
      <div class="col-sm-4">Margin: {{ cogsSalePriceMargin }}%</div>
    </div>


    <div class="row formula">
      <div class="col-sm-4">
        Cost of Goods <input type="number" class="inputBox" v-model="cogs3" />
      </div>
      <div class="col-sm-3">
        Markup <input type="number" class="inputBox" v-model="markup" /> %
      </div>
      <div class="col-sm-4 box3">Sale Price: {{ cogsMarkup }}</div>
    </div>


    <div class="row formula">
      <div class="col-sm-4">
        Cost of Goods <input type="number" class="inputBox" v-model="cogs4" />
      </div>
      <div class="col-sm-3">
        Sale Price <input type="number" class="inputBox" v-model="salePrice2" />
      </div>
      <div class="col-sm-4">Margin: {{ cogsSalePriceMarkup }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "home",
  data() {
    return {
      cogs1: 0,
      cogs2: 0,
      cogs3: 0,
      cogs4: 0,
      margin: 0,
      markup: 0,
      salePrice1: 0,
      salePrice2: 0,
    };
  },
  computed: {
    cogsMargin() {
      if (this.margin === 0) {
        return 0;
      } else {
        return this.cogs1 / (1 - this.margin / 100);
      }
    },
    cogsSalePriceMargin() {
      if (this.salePrice1 === 0) {
        return 0;
      } else {
        return ((this.salePrice1 - this.cogs2) / this.salePrice1) * 100;
      }
    },
    cogsMarkup() {
      if (this.markup === 0) {
        return 0;
      } else {
        return parseInt(this.markup / 100) * this.cogs3 + parseInt(this.cogs3);
      }
    },
  },
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
  border: 1px solid rgb(172, 172, 172);
  padding: 15px 2px;
  font-size: 22px;
  background-color: white;
  margin: 20px 20px 20px 0px;
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
