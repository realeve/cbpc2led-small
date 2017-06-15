<template>
  <div class="qrtip data-wrapper">
    <div class="qr-code">
      <div class="content"></div>
    </div>
    <div class="qr-text">
      <div class="wrap-title">参与留言</div>
      <div class="qr-info">扫描二维码关注“品质成钞”，点击『两周年留言』菜单进入留言。</div>
    </div>
  </div>
</template>

<script>
  export default {}

</script>

<style scoped lang="less">
  // .data-wrapper{
  //   border:none;
  // }
  @qrSize: 50px;
  .qrtip {
    height: @qrSize;
    width: 100%;
    display: flex;
    justify-content: flex-start;
    flex-direction: column;
  }

  .qr-code {
    background: #fff;
    width: @qrSize;
    margin-right: .5em;
  }

  .content {
    background-image: url('./img/qr.png');
    background-repeat: no-repeat;
    background-size: @qrSize @qrSize;
    width: @qrSize;
    height: @qrSize;
    box-shadow: 0 0 14px #195df3;
  }

  .text {
    width: 100%;
    display: flex;
    justify-content: flex-start;
    align-items: flex-start;
    text-overflow: ellipsis;
    white-space: nowrap;
    overflow: hidden;
  }

  .qr-text {
    width: 100%;
    max-width: 190px;
    margin-top:-10px;
    .wrap-title {
      color: #fff;
      font-size: 15px;
      height: 20px;
      .text;
    }
    .qr-info {
      color: #fff;
      font-size: 10px;
    }
  }

  .full-height {
    height: @qrSize;
  }

</style>
