<template>
  <div class="form-popup">
    
    <div class="cta-img" :style="inlineStyle">
       <h2 class="mt-5">{{ tagline }}</h2>
    </div>
    <div class="form-ctn">
      <h2>Get an Instant Quote</h2>
       <p>To get a personalised quote fill out form and we’ll get back to you.</p>
       <div id='crmWebToEntityForm' class='zcwf_lblLeft crmWebToEntityForm' style='background-color: white;color: black;max-width: 600px;'>
  <meta name='viewport' content='width=device-width, initial-scale=1.0'>
   <meta HTTP-EQUIV ='content-type' CONTENT='text/html;charset=UTF-8'>
<form action='https://crm.zoho.com/crm/WebToLeadForm' name=WebToLeads5345766000059706124 method='POST' onSubmit='javascript:document.charset="UTF-8"; return checkMandatory5345766000059706124()' accept-charset='UTF-8'>
 <input type='text' style='display:none;' name='xnQsjsdp' value='494948d118106026a8cc36236f116ef742d8513c2f869db6be604de04620f85e'></input> 
 <input type='hidden' name='zc_gad' id='zc_gad' value=''></input> 
 <input type='text' style='display:none;' name='xmIwtLD' value='07a3f6f26bd2426915b9c02c36b98748e2546b07df99cf35361578598979af53'></input> 
 <input type='text'  style='display:none;' name='actionType' value='TGVhZHM='></input>
 <input type='text' style='display:none;' name='returnURL' value='https://hppdev.com/thankyou' > </input>
	 <!-- Do not remove this code. -->
	 <input type='text' style='display:none;' id='ldeskuid' name='ldeskuid'></input>
	 <input type='text' style='display:none;' id='LDTuvid' name='LDTuvid'></input>
	 <!-- Do not remove this code. -->
<div class="two-feilds">
  <div class='zcwf_row'><div class='zcwf_col_fld'><input type='text' id='Last_Name' required placeholder="Name*" name='Last Name' maxlength='80'></input><div class='zcwf_col_help'></div></div></div>
<div class='zcwf_row'><div class='zcwf_col_fld'><input type='text' required placeholder="Email*" ftype='email' id='Email' name='Email' maxlength='100'></input><div class='zcwf_col_help'></div></div></div>
</div>
<div class="two-feilds">
  <div class='zcwf_row'><div class='zcwf_col_fld'><input type='text' required placeholder="Phone*" id='Phone' name='Phone' maxlength='30'></input><div class='zcwf_col_help'></div></div></div>
<div class='zcwf_row'><div class='zcwf_col_fld'><input type='number' min="200" @change="handleQuantityChange"  v-model="maxQty" required placeholder="Quantity MQ(200)*" id='LEADCF51' name='LEADCF51' maxlength='9'></input><span v-if="isvalid" style="font-size: 11px;
    color: red;">Minimum 200 | Great Savings on Larger Orders</span><div class='zcwf_col_help'></div></div></div>
</div>
<div class="two-feilds">
  <div class='zcwf_row'><div class='zcwf_col_fld'><select v-model="selected" class='zcwf_col_fld_slt mt-3' id='LEADCF1' name='LEADCF1'  >
			<option v-for="(item, index) in boxByType" :key="index" :value="item.name">{{item.name}}</option>
		</select><div class='zcwf_col_help'></div></div></div>
<div class='zcwf_row'><div class='zcwf_col_fld'><input type='text' id='Company' placeholder="Company Name" name='Company' maxlength='200'></input><div class='zcwf_col_help'></div></div></div>
</div>
<div style="display: none;" class='zcwf_row wfrm_fld_dpNn'><div class='zcwf_col_lab mt-2' style='font-size:12px; font-family: Arial; display: none;'><label for='LEADCF14'>Brand</label></div><div class='zcwf_col_fld'><select class='zcwf_col_fld_slt' id='LEADCF14' name='LEADCF14'  >
			<option value='-None-'>-None-</option>
		<option selected value='Half&#x20;Price&#x20;Packaging&#x20;US'>Half Price Packaging US</option>
			<option value='CBD&#x20;Box&#x20;Factory'>CBD Box Factory</option>
			<option value='The&#x20;Box&#x20;Factory'>The Box Factory</option>
		</select><div class='zcwf_col_help'></div></div></div>
<div style="display: none;" class='zcwf_row wfrm_fld_dpNn'><div class='zcwf_col_lab' style='font-size:12px; font-family: Arial; display: none;'><label for='LEADCF13'>Medium</label></div><div class='zcwf_col_fld'><select class='zcwf_col_fld_slt' id='LEADCF13' name='LEADCF13'  >
			<option value='-None-'>-None-</option>
		<option selected value='Custom&#x20;Quote&#x20;Form'>Custom Quote Form</option>
			<option value='Sample&#x20;Kit&#x20;Form'>Sample Kit Form</option>
			<option value='Popup&#x20;Quote&#x20;Form'>Popup Quote Form</option>
			<option value='Book&#x20;a&#x20;Call&#x20;Form'>Book a Call Form</option>
			<option value='Beat&#x20;The&#x20;Price&#x20;Form'>Beat The Price Form</option>
			<option value='Instant&#x20;Quote'>Instant Quote</option>
			<option value='Contact&#x20;Us&#x20;Form'>Contact Us Form</option>
			<option value='Request&#x20;Quote&#x20;Sidebar&#x28;TBF&#x29;'>Request Quote Sidebar&#x28;TBF&#x29;</option>
			<option value='Request&#x20;Quote&#x20;&#x28;TBF&#x29;'>Request Quote &#x28;TBF&#x29;</option>
			<option value='Product&#x20;Quote&#x20;&#x28;TBF&#x29;'>Product Quote &#x28;TBF&#x29;</option>
			<option value='Contact&#x20;US&#x20;&#x28;TBF&#x29;'>Contact US &#x28;TBF&#x29;</option>
			<option value='Contact&#x20;Us&#x20;&#x28;CPL&#x29;'>Contact Us &#x28;CPL&#x29;</option>
			<option value='Custom&#x20;Quote&#x28;CPL&#x29;'>Custom Quote&#x28;CPL&#x29;</option>
			<option value='Popup&#x20;Form&#x28;CPL&#x29;'>Popup Form&#x28;CPL&#x29;</option>
			<option value='Contact&#x20;Us&#x28;CBD&#x29;'>Contact Us&#x28;CBD&#x29;</option>
			<option value='Product&#x20;Quote&#x28;CBD&#x29;'>Product Quote&#x28;CBD&#x29;</option>
			<option value='Request&#x20;Quote&#x28;CBD&#x29;'>Request Quote&#x28;CBD&#x29;</option>
			<option value='Request&#x20;Quote&#x20;Sidebar&#x28;CBD&#x29;'>Request Quote Sidebar&#x28;CBD&#x29;</option>
			<option value='SMS&#x20;Marketing&#x20;KHI'>SMS Marketing KHI</option>
			<option value='Beat&#x20;Price'>Beat Price</option>
			<option value='Import'>Import</option>
			<option value='Chat'>Chat</option>
			<option value='Auto&#x20;Capture'>Auto Capture</option>
			<option value='CSR'>CSR</option>
			<option value='Outreach&#x20;Paid&#x20;Data'>Outreach Paid Data</option>
			<option value='Manual&#x20;Email&#x20;Outreach'>Manual Email Outreach</option>
			<option value='Instagram&#x20;Manual&#x20;Outreach'>Instagram Manual Outreach</option>
			<option value='Bob&#x20;LinkedIn&#x20;Outreach'>Bob LinkedIn Outreach</option>
			<option value='LinkedIn&#x20;Manual&#x20;Outreach'>LinkedIn Manual Outreach</option>
			<option value='Import-CSR'>Import-CSR</option>
		</select><div class='zcwf_col_help'></div></div></div>
<div class='zcwf_row' style="display: none;"><div class='zcwf_col_lab' style='font-size:12px; font-family: Arial; display:none'><label for='Street'>Street</label></div><div class='zcwf_col_fld'><input type='text' id='Street' name='Street' maxlength='250'></input><div class='zcwf_col_help'></div></div></div>
<div class='zcwf_row' style="display: none;"><div class='zcwf_col_lab' style='font-size:12px; font-family: Arial; display:none'><label for='City'>City</label></div><div class='zcwf_col_fld'><input :value="ip2loc_city" type='text' id='City' name='City' maxlength='100'></input><div class='zcwf_col_help'></div></div></div>
<div class='zcwf_row' style="display: none;"><div class='zcwf_col_lab' style='font-size:12px; font-family: Arial; display:none'><label for='Country'>Country</label></div><div class='zcwf_col_fld'><input :value="ip2loc_country" type='text' id='Country' name='Country' maxlength='100'></input><div class='zcwf_col_help'></div></div></div>
<div class='zcwf_row' style="display: none;"><div class='zcwf_col_lab' style='font-size:12px; font-family: Arial; display:none'><label for='State'>State</label></div><div class='zcwf_col_fld'><input :value="ip2loc_region" type='text' id='State' name='State' maxlength='100'></input><div class='zcwf_col_help'></div></div></div>
<div class='zcwf_row' style="display: none;"><div class='zcwf_col_lab' style='font-size:12px; font-family: Arial; display:none'><label for='LEADCF11'>IP</label></div><div class='zcwf_col_fld'><input :value="ip" type='text' id='LEADCF11' name='LEADCF11' maxlength='255'></input><div class='zcwf_col_help'></div></div></div>
<div class='zcwf_row' style="display: none;"><div class='zcwf_col_lab' style='font-size:12px; font-family: Arial; display:none'><label for='LEADCF10'>IP to ISP</label></div><div class='zcwf_col_fld'><input :value="ip2loc_isp" type='text' id='LEADCF10' name='LEADCF10' maxlength='255'></input><div class='zcwf_col_help'></div></div></div>
<div class='zcwf_row' style="display: none;"><div class='zcwf_col_lab' style='font-size:12px; font-family: Arial; display:none'><label for='LEADCF9'>IP to Org</label></div><div class='zcwf_col_fld'><input :value="ip2loc_org" type='text' id='LEADCF9' name='LEADCF9' maxlength='255'></input><div class='zcwf_col_help'></div></div></div>
<div class='zcwf_row' style="display: none;"><div class='zcwf_col_lab' style='font-size:12px; font-family: Arial; display:none'><label for='LEADCF16'>Page Url</label></div><div class='zcwf_col_fld'><input :value="page_url" type='text' id='LEADCF16' name='LEADCF16' maxlength='450'></input><div class='zcwf_col_help'></div></div></div>
<div class='zcwf_row' style="display: none;"><div class='zcwf_col_lab' style='font-size:12px; font-family: Arial; display:none'><label for='LEADCF15'>Fullpage Url</label></div><div class='zcwf_col_fld'><input :value="full_page_url" type='text' id='LEADCF15' name='LEADCF15' maxlength='450'></input><div class='zcwf_col_help'></div></div></div>
<div class="row" >
  <div  class='zcwf_row col-12'><div class='zcwf_col_fld'><textarea  placeholder="Provide detailed packaging specifications including dimensions, materials, weight restrictions, and design references and we'll get back to you with an instant quote." id='LEADCF35' name='LEADCF35'></textarea><div class='zcwf_col_help'></div></div></div>
  <div class='zcwf_row col-5 mob-file'>
    <div class='zcwf_col_fld'><div class='clearB'><input  type='file' class='zcwf_file' name='theFile' id='theFile5345766000059706124' multiple /><div class='zcwf_col_help'></div></div>
    </div>
    <p class="file-size">Attach Reference image or artwork (Max:20MB).</p>
  </div>
  <div class='zcwf_row col-7'> <div class='zcwf_col_lab'></div><div class='zcwf_col_fld'><div class='g-recaptcha' data-sitekey='6LfwhdkhAAAAAIw56jTra7exreIZpm-XxfJX50cn' data-theme='light' data-callback='rccallback5345766000059706124' captcha-verified='false' id='recap5345766000059706124'></div><div  id='recapErr5345766000059706124' style='font-size:12px;color:red;visibility:hidden;'>Captcha validation failed. If you are not a robot then please try again.</div></div></div>
</div>
<nuxt-link to="/bulk-order" class="bulk-order-link d-block text-center mt2 mb-1 text-decoration-none">Click Here for Bulk Order <img
              src="~/assets/icons/arrow-right-line.svg"
                alt="arrow right line"
            /></nuxt-link>
<b-button type="submit" :disabled="isvalid" class="cta-primary mt-0  mb-0 add-quote">
      <span v-show="!loading">Request a Quote</span> 
      <b-spinner v-show="loading"
        variant="danger"
      ></b-spinner>
    </b-button>
</form>
</div>

</div>

</div>
</template>

<script>
export default {
  name: "InstantQuotePopup",
  props:['boxByType', 'tagline', 'image', 'selected'],
  head() {
    return {
      script: [
        {
          type: 'text/javascript',
          id:'VisitorTracking',
          innerHTML: `
          var $zoho= $zoho || {};$zoho.salesiq = $zoho.salesiq || {widgetcode:'siq7554f5a6de5947a3bbb48ecbd8b715e435bf2a636fa2e2571eb445ab76f10a55', values:{},ready:function(){}};var d=document;s=d.createElement('script');s.type='text/javascript';s.id='zsiqscript';s.defer=true;s.src='https://salesiq.zoho.com/widget';t=d.getElementsByTagName('script')[0];t.parentNode.insertBefore(s,t);function trackVisitor5345766000059706151(){try{if($zoho){var LDTuvidObj = document.forms['WebToLeads5345766000059706151']['LDTuvid'];if(LDTuvidObj){LDTuvidObj.value = $zoho.salesiq.visitor.uniqueid();}var firstnameObj = document.forms['WebToLeads5345766000059706151']['First Name'];if(firstnameObj){name = firstnameObj.value +' '+name;}$zoho.salesiq.visitor.name(name);var emailObj = document.forms['WebToLeads5345766000059706151']['Email'];if(emailObj){email = emailObj.value;$zoho.salesiq.visitor.email(email);}}} catch(e){}}
          `
        },
        {
          type: 'text/javascript',
          innerHTML: `
          function validateEmail5345766000059706151()
{
  var form = document.forms['WebToLeads5345766000059706151'];
  var emailFld = form.querySelectorAll('[ftype=email]');
  var i;
  for (i = 0; i < emailFld.length; i++)
  {
    var emailVal = emailFld[i].value;
    if((emailVal.replace(/^\s+|\s+$/g, '')).length!=0 )
    {
      var atpos=emailVal.indexOf('@');
      var dotpos=emailVal.lastIndexOf('.');
      if (atpos<1 || dotpos<atpos+2 || dotpos+2>=emailVal.length)
      {
        alert('Please enter a valid email address. ');
        emailFld[i].focus();
        return false;
      }
    }
  }
  return true;
}

   function checkMandatory5345766000059706151() {
  var mndFileds = new Array('Name','Email','Phone');
  var fldLangVal = new Array('Name','Email', 'Phone');
  for(i=0;i<mndFileds.length;i++) {
    var fieldObj=document.forms['WebToLeads5345766000059706151'][mndFileds[i]];
    if(fieldObj) {
    if (((fieldObj.value).replace(/^\s+|\s+$/g, '')).length==0) {
     if(fieldObj.type =='file')
      { 
       alert('Please select a file to upload.'); 
       fieldObj.focus(); 
       return false;
      } 
    alert(fldLangVal[i] +' cannot be empty.'); 
              fieldObj.focus();
              return false;
    }  else if(fieldObj.nodeName=='SELECT') {
             if(fieldObj.options[fieldObj.selectedIndex].value=='-None-') {
      alert(fldLangVal[i] +' cannot be none.'); 
      fieldObj.focus();
      return false;
       }
    } else if(fieldObj.type =='checkbox'){
        if(fieldObj.checked == false){
      alert('Please accept  '+fldLangVal[i]);
      fieldObj.focus();
      return false;
       } 
     } 
     try {
         if(fieldObj.name == 'Last Name') {
      name = fieldObj.value;
           }
    } catch (e) {}
      }
  }
  trackVisitor5345766000059706151();
  if(!validateEmail5345766000059706151()){return false;}
  document.querySelector('.crmWebToEntityForm .formsubmit').setAttribute('disabled', true);
}

function tooltipShow5345766000059706151(el){
var tooltip = el.nextElementSibling;
var tooltipDisplay = tooltip.style.display;
if(tooltipDisplay == 'none'){
  var allTooltip = document.getElementsByClassName('zcwf_tooltip_over');
  for(i=0; i<allTooltip.length; i++){
    allTooltip[i].style.display='none';
  }
  tooltip.style.display = 'block';
}else{
  tooltip.style.display='none';
}
}
          `
        },
        {
          id: 'wf_anal',
          src: 'https://crm.zohopublic.com/crm/WebFormAnalyticsServeServlet?rid=07a3f6f26bd2426915b9c02c36b987483ff2872552d683c55f863b0e7718634agid494948d118106026a8cc36236f116ef742d8513c2f869db6be604de04620f85egid885e3c1045bd9bdcc91bdf30f82b5696gid14f4ec16431e0686150daa43f3210513&tw=61690b96c1d0471b638f31426f38e68aa67fb7ed6da86f32dc10ad817fe55a0a',
          defer: true
        },
        {
          src: 'https://www.google.com/recaptcha/api.js',
          defer: true
        }
      ]
    };
  },
  data: () => {
    return {
      dialog:false,
      loading: false,
      maxQty:'',
      isvalid: false,
      success: false,
      accessToken:"",
      ip:"",
      page_url: "",
      full_page_url: "",
      ip2loc_ip: "",
      ip2loc_isp: "",
      ip2loc_org:'',
      ip2loc_country: "",
      ip2loc_region: "",
      ip2loc_city:"",
      form_type:"beat_the_price",
    };
    
  },
  computed: {
    bgImage() {
      return require(`@/assets/images/primary-packaging/formimages/` + this.image);
    },
    inlineStyle() {
      return {
        backgroundImage: `url(${this.bgImage})`,
      };
    },
  },
  async mounted(){
      const ipResponse = await this.$axios.get('https://api.ipify.org?format=json');
      this.ip = ipResponse.data.ip;
      // Then get the geolocation data
      const geoResponse = await this.$axios.get(`http://api.ipstack.com/${this.ip}?access_key=9c0f5d88f80ce6b8c5d9843e10d85dbc`);
      let locationData = geoResponse.data;
      this.page_url = 'https://www.halfpricepackaging.com/' + this.$route.path;
      this.page_url = 'https://www.halfpricepackaging.com/' + this.$route.fullPath;
      this.ip2loc_ip =locationData.ip;
      this.ip2loc_isp = locationData.zip;
      this.ip2loc_org = locationData.zip;
      this.ip2loc_country = locationData.country_name;
      this.ip2loc_city = locationData.city;
      this.ip2loc_region = locationData.region_name;
  },
  methods:{
    handleQuantityChange() {
      if (this.maxQty < 200) {
        this.isvalid = true;
      }else{
        this.isvalid = false;

      }
    }
  }
};
</script>

<style lang="scss" scoped>
#crmWebToEntityForm.zcwf_lblLeft {
	width:100%;
	padding: 0px !important;
	margin: 0 auto;
	box-sizing: border-box;
}
.clearB{
  input{
    border-radius: 8px !important;
    background: #efefef;
    padding: 12px;
    cursor: pointer;
    width: 100% !important;
  }
  input:hover{
    background: #ef575c;
  }
}
.file-size{
  color: black;
    font-size: 12px;
    margin: auto;
    text-align: center;
    margin-bottom: 0px !important;
}
.form-popup{
  display: flex;
  justify-content: space-between;
  .zcwf_lblLeft .zcwf_row {
    margin: 8px 0px !important;
    width: 100%;
}
.zcwf_lblLeft .zcwf_col_fld input[type=text], input[type=number]{
	border-radius: 0px !important;
  border: none !important;
  border-bottom: 1px solid gray !important;
  width: 100% !important;
  min-height: 40px;
  margin-top: 5px;
  font-size: 14px;
  padding: 8px;
}
.zcwf_lblLeft .zcwf_col_fld textarea {
	border: none;
  width: 100%;
  height: 90px;
  font-size: 14px;
}
.zcwf_lblLeft .zcwf_col_fld {
    float: left;
    width: 100%;
    padding: 0px 6px 0px;
    position: relative;
    margin-top: 5px;
}
.zcwf_lblLeft {
    .zcwf_col_fld_slt{
    border-bottom: 1px solid #c0c6cc !important;
    border-style: none;
      border-bottom-style: none;
    float: left;
    line-height: 20px;
    max-width: 100%;
    min-width: 0;
    padding: 8px 0;
    resize: vertical;
    width: 100%;
    
  }
  .zcwf_col_fld_slt::-webkit-scrollbar {
  width: 7px;
}

/* Style the scrollbar thumb */
.zcwf_col_fld_slt::-webkit-scrollbar-thumb {
  background-color: #888;
  border-radius: 5px;
}

/* Style the scrollbar thumb when hovered */
.zcwf_col_fld_slt::-webkit-scrollbar-thumb:hover {
  background-color: #555;
}
  }

  .cta-img{
    flex-basis: 40%;
    background-size: cover;
    opacity: 1;
    margin: -16px;
    border-top-left-radius: 4px;
    border-bottom-left-radius: 4px;
      h2{
        text-align: center;
        font-size: 28px;
        color:#fff;
      }
  }
  .form-ctn {
    flex-basis: 60%;
    padding: 0px;
      h2 {
      font-size: 28px;
      text-align: center;
      }
      p{
        text-align: center;
      }
   form {

  .two-feilds{
    display: flex;
    gap: 10px;
    justify-content: space-between;
  }
}
}
}
@media (max-width:820px) {
  .form-popup{
.zcwf_lblLeft .zcwf_col_fld input[type=text], input[type=number]{
  width:100% !important;
}
  .cta-img{
    display: none;
  }
  .form-ctn {
    padding: 0px;
    flex-basis:100%;
    form {
      input {
        width: 150px;
      }
      .zcwf_col_lab{
        width: 150px;
      }
    }
  }
}
}
@media (max-width:480px) {

  .form-popup{
.zcwf_lblLeft .zcwf_col_fld input[type=text], input[type=number]{
  width:100% !important;
}
  .cta-img{
    display: none;
  }
  .form-ctn {
    padding: 0px;
    form {
      input {
        width: 150px;
      }
      .zcwf_col_lab{
        width: 150px;
      }
    }
  }
}
.col-7, .mob-file{
  max-width: 100%;
  flex-basis: 100%;
}
}
</style>