<template>
<div class="group-wrapper">
    <div class="card-group"  v-for="social in socials" :key="social.id">
      <div class="card-sm">
        <div class="head">
          <p>Views</p>
          <img src="../assets/icon-facebook.svg" alt="facebook icon">
        </div>
        <div class="numbers">
          <h1>{{  social.views }}</h1>
          <span>
            <img src="../assets/icon-up.svg" alt="">
            <p>{{ social.deltaViews }}%</p>
          </span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      socials: [
        {
          network: 'facebook',
          name: '@theo',
          followers: '1987',
          delta: '12',
          views: '87',
          likes: '52',
          deltaViews: '3',
          deltaLikes: '2'
        },
         {
          network: 'twitter',
          name: '@theo550',
          followers: '1044',
          delta: '99',
          views: '117',
          likes: '507',
          deltaViews: '303',
          deltaLikes: '557'
        },
        {
          network: 'instagram',
          name: '@theoinsta',
          followers: '11k',
          delta: '1099',
          views: '5462',
          likes: '52k',
          deltaViews: '2257',
          deltaLikes: '1375'
        },
        {
          network: 'youtube',
          name: '@theoYT',
          followers: '8239',
          delta: '144',
          views: '107',
          likes: '1407',
          deltaViews: '19',
          deltaLikes: '12'
        },
        ],
    }
  }
}
</script>

<style src="../style.css">

</style>