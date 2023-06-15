<template>
  <Form   @getPage="getPage" v-if="page == 'form'" />
  <Tables @getPage="getPage" v-if="page == 'table'" />
</template>

<script>
import Form from "./Form.vue";
import Tables from "./Tables.vue";

export default {
  name: "Index",
  components: {
    Form,
    Tables,
  },
  data() {
    return {
      page: "table",
    //   activeComponent: ["Table", "Form"],
    };
  },
  methods:{
    getPage(vlaue){
        this.page=vlaue
        
    }
  }
};
</script>

<style lang="scss" scoped></style>
