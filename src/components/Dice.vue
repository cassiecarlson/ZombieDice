<style scoped>
.table tbody tr > td.red {
  background-color: #D32F2F !important;
}

.table tbody tr > td.green {
  background-color: #43A047 !important;
}

.table tbody tr > td.yellow {
  background-color: #FFFF00 !important;
}
</style>

<template>
  <h2 class="text-center">Locked</h2>
  <table class="table table-hover table-striped">
    <thead>
    </thead>
    <tbody>
    <tr>
      <td v-for="dice in locked" class="{{dice.class}}">
          {{dice.result}}
      </td>
    </tr>
    </tbody>
  </table>

  <h2 class="text-center">Unlocked</h2>
  <table class="table table-hover table-striped">
    <thead>
    </thead>
    <tbody>
    <tr>
      <td v-for="dice in unlocked" class="{{dice.class}}">
          {{dice.result}}
      </td>
    </tr>
    </tbody>
  </table>
</template>

<script>
export default {
  data () {
    return {
      locked: [
        {
          result: 'shotgun',
          class: 'red'
        },
        {
          result: 'brains',
          class: 'green'
        },
        {
          result: 'brains',
          class: 'yellow'
        }
      ],
      unlocked: [
        {
          result: 'feet',
          class: 'green'
        },
        {
          result: 'feet',
          class: 'yellow'
        },
        {
          result: 'feet',
          class: 'red'
        }
      ]
    }
  }
}
</script>
