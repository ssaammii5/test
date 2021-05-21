<template>
  <div class="income-list">
    <IncomeItem v-for="x in props.state" :key="x.id" />
  </div>
</template>

<script>
import IncomeItem from "./IncomeItem";
export default {
  props: {
    state: Number,
  },
  components: {
    IncomeItem,
  },
  setup() {
    return {};
  },
};
</script>

<style scoped>
.income-list {
  margin-top: 30px;
  padding: 15px;
}
</style>
