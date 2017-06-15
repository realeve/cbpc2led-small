<template>
  <div>
    <full-image/>
    <v-header/>
    <flexbox :gutter="0" wrap="wrap" class="content">
      <flexbox-item :span="2/7">
        <v-left class="left-content" />
      </flexbox-item>
      <flexbox-item :span="3/7">
        <v-center class="center-content" />
      </flexbox-item>
      <flexbox-item :span="2/7">
        <v-right class="right-content" />
      </flexbox-item>
    </flexbox>
  </div>
</template>

<script>
  import FullImage from './IFullImage/index'
  import VHeader from './Header/';
  import VCenter from './Center.vue';
  import VLeft from './Left.vue';
  import VRight from './Right.vue';

  import {
    Flexbox,
    FlexboxItem
  } from 'vux';

  export default {
    components: {
      Flexbox,
      FlexboxItem,
      FullImage,
      VHeader,
      VLeft,
      VCenter,
      VRight
    }
  }

</script>
<style scoped lang="less">
  @div-offset: 310px;
  .content {
    margin-top: -@div-offset;
    color: #fff;
  }

  .center-content {
    padding: 230px 10px 0 20px;
  }

  .left-content {
    padding: 140px 15px 0px 5px;
  }

  .right-content {
    padding: 210px 5px 0px 0px;
  }

</style>
