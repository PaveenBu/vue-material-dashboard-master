<template>
  <div class="content">
    <div class="md-layout">
      
      
      
      
      <div
        class="md-layout-item md-medium-size-100 md-xsmall-size-100 md-size-50"
      >
        <md-card>
          <md-card-header data-background-color="red">
            <h4 class="title">Assets Status</h4>
            <p class="category">Last borrowed</p>
          </md-card-header>
          <md-card-content>
            <ordered-table table-header-color="red"></ordered-table>
          </md-card-content>
        </md-card>
      </div>
      
    </div>
  </div>
</template>

<script>
import {
  StatsCard,
  ChartCard,
  NavTabsCard,
  NavTabsTable,
  OrderedTable,
} from "@/components";

export default {
  components: {
    OrderedTable,
  },
  data() {
    return {
      
    };
  },
};
</script>
