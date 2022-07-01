<template>
    <table>
        <tr v-for="d in data" :key="d.index">
            <td>{{d.index}}</td>
            <td>{{d._id}}</td>
            <td>{{d.guid}}</td>
        </tr>
    </table>
</template>

<script>
    import Data from './data.json'
    export default {
        name: 'App',
        data() {
            return {
                data: Data
            };
        }
    }
</script>

<style>
  @import './Own.css';
</style>
