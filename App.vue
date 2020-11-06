<template>
  <div id="app">
    <b-table :data="data" :columns="columns"></b-table>
    <AddTodo/>
  </div>
</template>

<script>
import AddTodo from './components/AddTodo.vue'

export default {
  name: 'App',
  components: {
    AddTodo
  },
  data() {
            return {
                data: [
                    { 'id': 1, 'plant': 'Ivory Towers', 'latin': 'Crassula perforata', 'date': '2016-10-15 13:43:27', 'stock': 'yes' },
                    { 'id': 2, 'plant': 'Red Heuff', 'latin': 'Sempervivum heuffelii', 'date': '2016-12-15 06:00:53', 'stock': 'yes' },
                    { 'id': 3, 'plant': 'String of Pearls', 'latin': 'Senecio rowleyanus', 'date': '2016-04-26 06:26:28', 'stock': 'no' },
                    { 'id': 4, 'plant': 'Thimble Cactus', 'latin': 'Mammillaria gracilis', 'date': '2016-04-10 10:28:46', 'stock': 'yes' },
                    { 'id': 5, 'plant': 'Torch Cactus', 'latin': 'Echinopsis spachiana', 'date': '2016-12-06 14:38:38', 'stock': 'no' }
                ],
                columns: [
                    {
                        field: 'id',
                        label: 'ID',
                        width: '40',
                        numeric: true
                    },
                    {
                        field: 'plant',
                        label: 'Plant',
                    },
                    {
                        field: 'latin',
                        label: 'Latin',
                    },
                    {
                        field: 'date',
                        label: 'Date',
                        centered: true
                    },
                    {
                        field: 'stock',
                        label: 'Stock',
                    }
                ]
            }
        }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  max-width: 600px;
  margin: 60px auto;
}
</style>
