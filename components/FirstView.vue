<template>
  <div class="FirstContent">
    <CCCLogo class="Logo" />
    <v-card class="FirstView-Card" elevation="0" width="80%">
      <v-card-title class="FirstView-Card-Copy">
        <span><span class="Marker">学生</span>がつくる</span>
        <span><span class="Marker">未来</span>のカタチ</span>
      </v-card-title>
      <v-card-text style="text-align: left" class="FirstView-Card-Concept">
        行きたかったインターンにいけない。<br />
        時間はたくさんあるのに、好きなことができない。<br />
        身近の課題は見えているけれど、一人ではどうにもならない。<br />
        <br />
        だから、私は仲間とともに挑戦する。<br />
      </v-card-text>
    </v-card>
  </div>
</template>

<script>
import CCCLogo from '@/static/CCCLogo.svg'
export default {
  name: 'FirstView',
  components: {
    CCCLogo,
  },
}
</script>

<style lang="scss" scoped>
.Logo {
  width: 65%;
  height: auto;
}
.FirstView-Card {
  margin-right: auto;
  margin-left: auto;
  padding: 30px 50px;
  @media (max-width: 750px) {
    padding: 10px;
  }
  &-Copy {
    font-family: $font-ja;
    font-size: 35px;
    font-weight: 900;
    line-height: 1.51;
    letter-spacing: 2.33px;
    color: $indigo-1;

    .Marker {
      background: linear-gradient(transparent 60%, #ffd500 30%);
    }
  }

  &-Concept {
    font-family: $font-ja;
    font-size: 16px;
    font-weight: 700;
    line-height: 1.94;
    letter-spacing: 1px;
    color: $indigo-1 !important;
    margin-top: 20px;
  }
}
</style>
