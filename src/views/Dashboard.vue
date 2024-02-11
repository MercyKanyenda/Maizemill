<script setup>
import Nav from "../components/Nav.vue";
import Barchart from "../components/Barchart.vue";
import Card from "../components/common/Card.vue";
</script>

<template>
  <div>
    <Nav />
    <main>
      <div class="dash_header">
        <h4 class="text-h4">Dashboard</h4>
        <div>
          <v-btn> Add To Inventory </v-btn>
          <v-btn> Sale </v-btn>
        </div>
      </div>
      <div class="content">
        <div class="top_content">
          <div class="top_content_left">
            <Barchart />
          </div>
          <div class="top_content_right">
            <Card title="Total Revenue" amount="35,000,000" />
            <Card title="Total KGs" amount="65" />
          </div>
        </div>
        <v-card>
          <v-card-title>
            Recent Activities
          </v-card-title>
        </v-card>
      </div>
    </main>
  </div>
</template>

<style>
.dash_header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 2rem;
}

.top_content_left{
  flex: 70%;
}

.top_content_right{
  flex: 30%;
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.top_content {
  display: flex;
  gap: 1rem;
  justify-content: space-between;
}
</style>
