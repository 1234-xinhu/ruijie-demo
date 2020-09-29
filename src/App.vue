<template>
  <div id="app">
    <Head><img  class = "head-img" src="https://app.ruijienetworks.com:9443/admin/resources/skin/default/images/enquiry/banner-0526-pc.png" alt=""></Head>
    <FormData/>
    <Footer class = "footer-item">
      <div ><img class = "footer-img" src="https://app.ruijienetworks.com:9443/admin/resources/skin/default/images/enquiry/cloud.png" alt=""></div>
      <div ><span class = "footer-text">Try login to check out your Ruijie Cloud account</span></div>
      <div ><a  class = "footer-btn google-play" href="https://play.google.com/store/apps/details?id=cn.com.ruijie.cloudapp"></a></div>
      <div ><a  class = "footer-btn app-store"  href="https://itunes.apple.com/us/app/ruijie-cloud/id1423429270?ls=1&mt=8"></a></div>
    </Footer>
  </div>
</template>

<script>
import Head from './components/Head'
import FormData from './components/FormData'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    Head,
    FormData,
    Footer
  }
}
</script>

<style>
.head-img {
  display: flex;
  width: 95%;
  height: 400px;
  margin: 0 auto;
}


.footer-item div {
  flex: 1;
}


.footer-img {
  width: 80px;
  height: 80px;
}

.footer-btn {
      display: inline-block;
      width: 180px;
      border: 1px solid #8c8c8c;
      height: 48px;
      border-radius: 14px;
      cursor: pointer;
}

.google-play {
  background: url(https://app.ruijienetworks.com:9443/admin/resources/skin/default/images/enquiry/google-play.png) no-repeat center;
}

.app-store {
  background: url(https://app.ruijienetworks.com:9443/admin/resources/skin/default/images/enquiry/app-store.png) no-repeat center;
}


.footer-text {
  margin-left: -100px;
  color: #8c8c8c;
  font-family: Arial, '微软雅黑', sans-serif !important;
}
</style>
