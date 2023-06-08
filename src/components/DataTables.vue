<template>
    <n-data-table :columns="columns" :data="data" />
</template>
  
  <script>
  import { defineComponent, ref } from "vue";
  import { NDataTable } from "naive-ui";
  
  const createColumns = () => {
    return [
        {
        title: "No",
        key: "no"
        },
        {
        title: "Title",
        key: "title"
        },
        {
        title: "Length",
        key: "length"
        },
        {
        title: "Action",
        key: "actions"
        }
    ];
  };
  
  export default {
    components: {
        NDataTable
  },
    setup() {
      return {
        data: ref([
            { no: 3, title: "Wonderwall", length: "4:18" },
            { no: 4, title: "Don't Look Back in Anger", length: "4:48" },
            { no: 12, title: "Champagne Supernova", length: "7:27" }
        ]),
        columns: createColumns()
      };
    }
  };
  </script>