<template>
  <div class="sas-breadcrumb">
    <el-breadcrumb  :separator="separator" >
      <slot></slot>
    </el-breadcrumb>  
  </div>
</template>
<script>
  export default {
    name: 'LvxBreadcrumb',
    data: function () {
      return {
        separator: '/'
      };
    },
    props: {
    }
  };
</script>
<style lang="scss" type="text/scss" >
  .sas-breadcrumb{
    .el-breadcrumb__item{
      .el-breadcrumb__inner{
        color: #d9d9d9;
        font-weight: normal;
      }
      &:last-child{
        .el-breadcrumb__inner{
          color: #333;
        }
      }
    }
  }
</style>