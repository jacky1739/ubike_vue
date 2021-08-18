<template>
  <div class="container">
    <div class="row no-gutters">
      <div class="col-sm-3 d-flex p-2 bg-white">
        <label for="city" class="col-form-label mr-2 text-right">縣市</label>
        <div class="flex-fill">
          <select id="city" class="form-control">
            <!-- 製作下拉選單 -->
            <option value="台北市">台北市</option>
          </select>
        </div>
      </div>
      <div class="d-flex col-sm-3 p-2 bg-white">
        <label for="dist" class="col-form-label mr-2 text-right">地區</label>
        <div class="flex-fill">
          <select id="dist" class="form-control">
            <!-- 製作下拉選單 -->
            <option value="中正區">中正區</option>
          </select>
         </div>
      </div>
      <div class="col-sm-9">
        <div id="map"></div>
      </div>
    </div>
  </div>
</template>

<script>
// import cityName from '@/assets/cityName.json'

export default {
  data () {
    return {
      cityName: '',
      select: {
        city: '台北市',
        dist: '中正區'
      }
    }
  }
}
</script>
