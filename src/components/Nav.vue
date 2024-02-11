<template>
   
        <nav class="navigation">
            <h2>Logo</h2>
            <div class="navigation-items">
                <router-link to="/">Dashboard</router-link>
                <router-link to="/inventory">Inventory</router-link>
                <router-link to="/sales">Sales</router-link>
            </div>
            <v-btn class="log">
                Log Out
            </v-btn>
        </nav>
</template>
<style scoped>
    .navigation{
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 3rem;
    }
    .navigation-items{
        display: flex;
        gap: 1rem;
    }
    .log{
        background-color: rgb(203, 203, 201);
        color: rgb(0, 0, 0);
        height: 25px;
        width: 80px;
    }
    .buttons{
        display: flex;
        justify-content: space-between;
        justify-content: flex-end;
        padding-top: 40px;
    }
    .buttons > .v-btn {
  /*  margin-right: 10px; /* Adjust the value as needed */
    background-color: rgb(186, 194, 190); /* Change background color */
    color: rgb(0, 0, 0); /* Change text color */
    height: 27px; /* Adjust height */
}
    .buttons > .v-btn:not(:last-child) {
    margin-right: 20px; /* Adjust the value as needed */
    } 
</style>