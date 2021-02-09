<template>
  <div class="home container-sm">
    <div class="row formula">
      <div class="col-sm-4 box1">
        Cost of Goods <input type="number" class="inputBox" v-model="cogs" />
      </div>
      <div class="col-sm-3 box2">
        Margin <input type="number" class="inputBox" v-model="margin" /> %
      </div>
      <div class="col-sm-4 box3">Sale Price: {{ cogsMargin }}</div>
    </div>
    <div class="row formula">
      <div class="col-sm-4 box1">
        Cost of Goods <input type="number" class="inputBox" v-model="cogs" />
      </div>
      <div class="col-sm-3 box2">
        Margin <input type="number" class="inputBox" v-model="margin" /> %
      </div>
      <div class="col-sm-4 box3">Sale Price: {{ cogsMargin }}</div>
    </div>
    <div class="row formula">
      <div class="col-sm-4 box1">
        Cost of Goods <input type="number" class="inputBox" v-model="cogs" />
      </div>
      <div class="col-sm-3 box2">
        Margin <input type="number" class="inputBox" v-model="margin" /> %
      </div>
      <div class="col-sm-4 box3">Sale Price: {{ cogsMargin }}</div>
    </div>
    <div class="row formula">
      <div class="col-sm-4 box1">
        Cost of Goods <input type="number" class="inputBox" v-model="cogs" />
      </div>
      <div class="col-sm-3 box2">
        Margin <input type="number" class="inputBox" v-model="margin" /> %
      </div>
      <div class="col-sm-4 box3">Sale Price: {{ cogsMargin }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "home",
  data() {
    return {
      cogs: 0,
      margin: 0,
      salePrice: 0,
    };
  },
  computed: {
    cogsMargin() {
      if (this.margin === 0) {
        return 0;
      } else {
        return this.cogs / (1 - this.margin / 100);
      }
    },
    cogsSalePrice() {
      if (this.margin === 0) {
        return 0;
      } else {
        return this.cogs / (1 - this.margin / 100);
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
