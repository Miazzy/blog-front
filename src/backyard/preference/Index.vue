<template>
	<div class="backyard-preference">
		<div class="row">
			<div class="col-lg-12">
				<div class="pedia-navigation">
					<span class="item active">网站偏好</span>
          <span class="tool">
            <router-link class="btn btn-sm btn-primary" to="/by/preference/edit">
              <i class="fa fa-pencil"></i>
              修改
            </router-link>
          </span>
        </div>
			</div>
      <div class="col-xs-12">
        <div class="mt10 bg-white br4 border">
          <div class="row p10 border-bottom">
            <div class="col-md-2 col-sm-2 col-xs-4 bold">
              网站名称
            </div>
            <div class="col-md-10 col-sm-10 col-xs-8">
              {{preference.name}}
            </div>
          </div>

          <div class="row p10 border-bottom">
            <div class="col-md-2 col-sm-2 col-xs-4 bold">
              logo
            </div>
            <div class="col-md-10 col-sm-10 col-xs-8" v-if="preference.logoUrl">
              <img :src="preference.logoUrl" alt="logo" class="tankImg">
            </div>
          </div>

          <div class="row p10 border-bottom">
            <div class="col-md-2 col-sm-2 col-xs-4 bold">
              favicon
            </div>
            <div class="col-md-10 col-sm-10 col-xs-8" v-if="preference.faviconUrl">
              <img :src="preference.faviconUrl" alt="favicon" class="tankImg">
            </div>
          </div>


          <div class="row p10 border-bottom">
            <div class="col-md-2 col-sm-2 col-xs-4 bold">
              菜单一
            </div>
            <div class="col-md-10 col-sm-10 col-xs-8">
              {{preference.menuName1}}
            </div>
          </div>

          <div class="row p10 border-bottom">
            <div class="col-md-2 col-sm-2 col-xs-4 bold">
              菜单一Url
            </div>
            <div class="col-md-10 col-sm-10 col-xs-8">
              {{preference.menuUrl1}}
            </div>
          </div>

          <div class="row p10 border-bottom">
            <div class="col-md-2 col-sm-2 col-xs-4 bold">
              菜单二
            </div>
            <div class="col-md-10 col-sm-10 col-xs-8">
              {{preference.menuName2}}
            </div>
          </div>

          <div class="row p10 border-bottom">
            <div class="col-md-2 col-sm-2 col-xs-4 bold">
              菜单二Url
            </div>
            <div class="col-md-10 col-sm-10 col-xs-8">
              {{preference.menuUrl2}}
            </div>
          </div>

          <div class="row p10 border-bottom">
            <div class="col-md-2 col-sm-2 col-xs-4 bold">
              菜单三
            </div>
            <div class="col-md-10 col-sm-10 col-xs-8">
              {{preference.menuName3}}
            </div>
          </div>

          <div class="row p10 border-bottom">
            <div class="col-md-2 col-sm-2 col-xs-4 bold">
              菜单三Url
            </div>
            <div class="col-md-10 col-sm-10 col-xs-8">
              {{preference.menuUrl3}}
            </div>
          </div>

          <div class="row p10 border-bottom">
            <div class="col-md-2 col-sm-2 col-xs-4 bold">
              菜单四
            </div>
            <div class="col-md-10 col-sm-10 col-xs-8">
              {{preference.menuName4}}
            </div>
          </div>

          <div class="row p10 border-bottom">
            <div class="col-md-2 col-sm-2 col-xs-4 bold">
              菜单四Url
            </div>
            <div class="col-md-10 col-sm-10 col-xs-8">
              {{preference.menuUrl4}}
            </div>
          </div>

          <div class="row p10 border-bottom">
            <div class="col-md-2 col-sm-2 col-xs-4 bold">
              菜单五
            </div>
            <div class="col-md-10 col-sm-10 col-xs-8">
              {{preference.menuName5}}
            </div>
          </div>

          <div class="row p10 border-bottom">
            <div class="col-md-2 col-sm-2 col-xs-4 bold">
              菜单五Url
            </div>
            <div class="col-md-10 col-sm-10 col-xs-8">
              {{preference.menuUrl5}}
            </div>
          </div>

          <div class="row p10 border-bottom">
            <div class="col-md-2 col-sm-2 col-xs-4 bold">
              底部文字1
            </div>
            <div class="col-md-10 col-sm-10 col-xs-8">
              <span v-html="preference.footerLine1"></span>
            </div>
          </div>

          <div class="row p10 border-bottom">
            <div class="col-md-2 col-sm-2 col-xs-4 bold">
              底部文字2
            </div>
            <div class="col-md-10 col-sm-10 col-xs-8">
              <span v-html="preference.footerLine2"></span>
            </div>
          </div>

        </div>

      </div>
		</div>

	</div>
</template>

<script>
  export default {
    name: 'index',
	  data(){
      return{
				preference: this.$store.state.preference
      }
	  },
	  methods:{

	  },
	  mounted(){
	  }
  }
</script>

<style lang="less" rel="stylesheet/less">
	.backyard-preference{
		.tankImg{
			max-height: 100px
		}
	}
</style>
