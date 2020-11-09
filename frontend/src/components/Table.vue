<template>
  <div>
    <!-- <b-table striped hover :items="items"></b-table> -->
 <b-table striped hover :items="items.data" :fields="fields"> </b-table>
  </div>
  
</template>

<script>
import axios from 'axios';

  export default {
   data() {
      return {
        fields: ['_id','name', 'email', 'food', 'create_date'],
        items: [], 
        
      }
    },
    created(){
    axios.get('http://localhost:8081/api/contacts').then(res =>{this.items = res.data, console.log(this.items.data) })
    .catch(err => console.log(err))
   }
  }
</script>