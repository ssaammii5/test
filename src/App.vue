<template>
  <Header :totalIncome="totalAmount" />
  <Form />
  <IncomeList :state="num" />
</template>

<script>
import { ref } from "vue";
import Header from "./components/Header";
import Form from "./components/Form";
import IncomeList from "./components/IncomeList";
export default {
  name: "App",
  components: {
    Header,
    Form,
    IncomeList,
  },
  setup() {
    let totalAmount = ref(500546);
    let num = ref(5);
    return {
      totalAmount,
      num,
    };
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Fira Sans", sans-serif;
}
body {
  background: #eee;
}
</style>
