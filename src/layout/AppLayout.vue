<template>
   
<div>
    <nav>
        <h2>Logo</h2>
        <v-card>
            <router-link to="/">Dashboard</router-link>
            <router-link to="/inventory">Inventory</router-link>
            <router-link to="/sales">Sales</router-link>
        </v-card>
    </nav>
    <component :is="this.$route.meta.layoutComponent">
<slot/>
    </component>
</div>
    

</template>