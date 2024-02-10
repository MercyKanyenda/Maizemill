<template>
   
        <nav class="navigation">
            <h2>Logo</h2>
            <div class="navigation-items">
                <router-link to="/">Dashboard</router-link>
                <router-link to="/inventory">Inventory</router-link>
                <router-link to="/sales">Sales</router-link>
            </div>
            <v-btn>
                Log Out
            </v-btn>
        </nav>
        
</template>
<style scoped>
    .navigation{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .navigation-items{
        display: flex;
        gap: 1rem;
    }
</style>