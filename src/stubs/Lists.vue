<template>
  <a-layout-content :style="{ padding: '0 50px', marginBottom: '50px' }">
    <div :style="{ background: '#fff', padding: '24px', minHeight: '280px' }">
      <CreateListModal />
      <div :style="{ marginBottom: '30px' }" class="gutter-example">
        <template v-for="key in 3">
          <a-row :key="key" :gutter="16">
            <template v-for="key in 4">
              <a-col :key="key" class="gutter-row" :span="6">
                <div class="gutter-box">
                  <Card />
                </div>
              </a-col>
            </template>
          </a-row>
        </template>
      </div>
      <Pagination />
    </div>
  </a-layout-content>
</template>

<script>
import Card from "./Card.vue";
import Pagination from "./Pagination.vue";
import CreateListModal from "../stubs/CreateListModal.vue";

export default {
  name: "Lists",
  components: {
    Card,
    Pagination,
    CreateListModal,
  },
};
</script>
