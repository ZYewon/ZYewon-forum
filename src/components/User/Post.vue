<template>
  <div class="fly-panel fly-panel-user" pad20>
    <div class="layui-tab layui-tab-brief">
      <ul class="layui-tab-title">
        <li>
          <router-link :to="{ name: 'mypost' }">我的发帖</router-link>
        </li>
        <li>
          <router-link :to="{ name: 'mycollection' }">我收藏的贴</router-link>
        </li>
      </ul>

      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import Editor from "../Editor";

export default {
  components: { Editor },
};
</script>

<style lang="less" scoped></style>
