<template>
<div class="overall-panel">
<h2>Overall Results</h2>

<table>
   <thead>
     <tr>
       <th>Pos</th>
       <th>Racer</th>
       <th>January</th>
       <th>February</th>
       <th>March</th>
       <th>April</th>
       <th>May</th>
       <th>June</th>
       <th>July</th>
       <th>August</th>
       <th>September</th>
       <th>October</th>
       <th>November</th>
       <th>December</th>
       <th>Total Points</th>
     </tr>
   </thead>
   <tbody>
    <tr v-for='entry in results'>
      <td>{{entry.position}}</td>
      <td>{{entry.name}}</td>
      <td v-for='month in entry.months'>{{month}}</td>
      <td>{{entry.total}}</td>
    </tr>
   </tbody>
</table>
</div>
</template>

<script>
export default {
  data() {
    return {
      results: [
        {
          position: 1,
          name: 'Mike R.',
          months: [12, 11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1],
          total: 150,
        },
        {
          position: 2,
          name: 'Mark S.',
          months: [12, 11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1],
          total: 150,
        },
      ],
    };
  },
};
</script>

<style>
.overall-panel {
  border: 2px solid red;
}

table, th, td {
  border: 1px solid black;
}

table {
  width: 100%;
}

</style>
