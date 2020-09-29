<template>
  <div class = "enquery-container">
    <h2 class="enquiry-title">Welcome to Attend Our Online Workshop</h2>
	<h3 class="enquiry-sub-title">Local Language | Online Presentation</h3>
    <div class="form">
        <ul class = "form-box">
            <li>       
                <div class = "enquiry-row">
                    <div class="enquery-left">
                        <span class = "enquiry-wrap">Country/Region</span>
                    </div>
                    <div class="enquiry-right">
                        <a-select default-value="China" style = "width: 320px;height: 42px" > 
                        <a-select-option
                            :value="item"
                            v-for="item in country"
                            :key="item"
                        >{{item}}
                        </a-select-option>
                        </a-select>
                    </div>
                </div>
            </li>
            <li>
                <div class = "enquiry-row">
                    <div class = "schedule-left">
                       <span class = "enquiry-wrap">Schedule</span> 
                       <p class = "tip">Please choose a schedule you are interested</p>
                    </div>
                   <div class="schedule-right">
                        <p>
                            Please leave your contact information below. Instant email notice to you as soon as events scheduled.
                        </p>
                   </div>
                </div>
            </li>
            <li>
                 <div class = "enquiry-row">
                    <div class="enquiry-left">
                        <span class = "enquiry-wrap">Name</span>
                    </div>
                    <div class="enquiry-right">
                        <a-input style = "height: 42px;width: 320px"/>
                    </div>
                </div>
            </li>
            <li>
                 <div class = "enquiry-row">
                    <div class="enquiry-left">
                        <span class = "enquiry-wrap">Emailn</span>
                    </div>
                    <div class="enquiry-right">
                        <a-input  style = "width: 320px;height: 42px" />
                    </div>
                </div>
            </li>
            <li>
                 <div class = "enquiry-row">
                    <div class="enquiry-left">
                        <span class = "enquiry-wrap">Job Title</span>
                    </div>
                    <div class="enquiry-right">
                        <a-select default-value="--Select Your Division--" style = "width: 320px;height: 42px" > 
                        <a-select-option
                            :value="item"
                            v-for="item in option"
                            :key="item"
                        >{{item}}
                        </a-select-option>
                        </a-select>
                    </div>
                </div>
            </li> 
            <li>
                <div class="submit">
                    <a-button class="submit-btn" type="primary" >Submit </a-button>
                </div>
            </li>
        </ul>
    </div>
  </div>
</template>

<script>
var country = ['--Select','Bahrain','Cambodia','China','China Hong Kong'];
var option = ['--Select Your Division--','owner','sales','Product/Marketing','Technical','Ruijie VAD/Sub-D/Ruijie Staff']
export default {
  name: 'FormData',
  data() {
      return {
      country: country,
      option: option
    };
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.enquiry-title {
    margin-bottom: 42px;
    text-align: center;
    font-size: 42px;
}


.enquiry-sub-title {
    margin-bottom: 42px;
    text-align: center;
    font-size: 24px;
    color: #8c8c8c;
}

.form-box li {
    list-style: none;
}


.form {
    width: 480px;
    margin: 0 auto;
}

.form-box {
    width: 100%;
    position: relative;

}

.enquiry-wrap {
    line-height: 42px;
    width: 160px;
    padding-right: 16px;
    text-align: right;
    font-size: 16px;
    display: inline-block;
    color: #8c8c8c;
}

.enquiry-row {
    display: flex;
    width: 480px;
    margin-bottom: 20px;
}


.enquery-container {
    background-color: rgb(252, 252, 250);
}

.enquery-left {
    width: 160px;
    height: 42px;
    text-align: left;
}

.enquery-right {
    width: 320px;
    height: 42px;
}

.submit {
    width: 320px;
    height: 88px;
    margin-left: 160px;
}

.submit-btn {
    width: 100%;
    height: 56px;

}

.schedule-left,
.schedule-right {
    height: 70px;
}

.tip {
    font-size: 12px;
    line-height: 1.5;
    color: #bfbfbf;
    margin-top: -8px;
    text-align: right;
    margin-right: 18px;
}
</style>
