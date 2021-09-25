<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <v-avatar size="200">
          <v-img :src="'http://q1.qlogo.cn/g?b=qq&nk='+social[2].number+'&s=640'"/>
        </v-avatar>
      </v-col>

      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          这里是 HikariLan 贺兰星辰😀
        </h1>

        <p class="subheading font-weight-regular">
          一个普通的学生，业余开发者，业余-业余运维，喜欢折腾新事物
        </p>

        <v-row justify="center">
          <div v-for="(it,i) in social" :key="i" style="padding: 5px">
            <v-btn
                :key="i"
                link="link"
                :href="it.link"
                outlined
                rounded
                x-large
            >{{ it.name }}
            </v-btn>
          </div>
        </v-row>
      </v-col>


    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'HelloWorld',

  data: () => ({
        social: [{
          name: "主页",
          link: "#"
        }, {
          name:"博客",
          link: "https://my.minecraft.kim"
        },
          {
            name: "QQ",
            link: "tencent://message/?uin=2191023046",
            number: 2191023046
          }, {
            name: "知乎",
            link: "https://www.zhihu.com/people/shaokeyibb"
          }, {
            name: "B站",
            link: "https://space.bilibili.com/29367276"
          }, {
            name: "GitHub",
            link: "https://github.com/shaokeyibb"
          }],
      }
  ),
}
</script>
