<template>
  <div class="about">
    <v-container style="max-width: 100%!important;">
      <v-tabs>
        <v-tab>
          文章/视频抽奖
        </v-tab>
        <v-tab-item>
          <ACDraw />
        </v-tab-item>
      </v-tabs>
    </v-container>
  </div>
</template>

<script>
import { formatDate } from '@/utils/timeFormat'
import ACDraw from '@/components/Fun/ACDraw.vue'

export default {
  data() {
    return {
    }
  },
  components: {
    ACDraw
  },
  filters: {
    formatDate(time) {
      let date = new Date(time)
      return formatDate(date, 'yyyy-MM-dd hh:mm')
    }
  },
  created() {
  },
  methods: {
  }
}
</script>