<template>
  <div class="service">
    <Navbarportion />
    <div class="service_back">
      <p class="text_1 text_p">Services that create identities, build brands, and get results</p>
    </div>
    <b-container>
        <h3 class="text-center text-capitalize mt-4">our services</h3>
        <div class="line"></div>
        <div class="line_2"></div>
        <p class="text-center text_2">We produce beautifully creative solutions that transcend business goals.</p>

         <b-row class="mt-5 content_align">
              <b-col>
                  <div class="service_area">
                      <div class="img_graphic"><label class="icon_portion"><img src="../static/marketing_img.png" class="images"  alt=""></label> </div>
                      <h5>branding marketing</h5>
                      <p class="text_1">Brand marketing is promoting a brand's products or services in a way that elevates the brand as a whole. </p>
                  </div>
              </b-col>
              <b-col>
                   <div class="service_area">
                      <div class="img_graphic"><label class="icon_portion"><img src="../static/graphic_design.png" class="images"  alt=""></label> </div>
                      <h5>Graphic design</h5>
                      <p class="text_1">2D Design is the most common technique used for the UI design we produce at our studio.</p>
                  </div>
              </b-col>
              <b-col>
                   <div class="service_area">
                      <div class="img_graphic"><label class="icon_portion"><img src="../static/web_img.png" class="images"  alt=""></label> </div>
                      <h5>web design & seo</h5>
                      <p class="text_1">It provides you with a customized website design that's perfect for your business or personal site.</p>
                  </div>
              </b-col>
          </b-row>
          <b-row class="mt-4 content_align">
              <b-col>
                  <div class="service_area">
                      <div class="img_graphic"><label class="icon_portion"><img src="../static/bulk_img.png" class="images"  alt=""></label> </div>
                      <h5>bulk sms </h5>
                      <p class="text_1">It refers to businesses sending SMS to one or more recipients via bulk SMS service providers such as Textlocal. </p>
                  </div>
              </b-col>
              <b-col>
                   <div class="service_area">
                      <div class="img_graphic"><label class="icon_portion"><img src="../static/app_img.png" class="images"  alt=""></label> </div>
                      <h5>mobile app</h5>
                      <p class="text_1">A Mobile app is a software application developed specifically for use on small, wireless computing devices</p>
                  </div>
              </b-col>
              <b-col>
                   <div class="service_area">
                      <div class="img_graphic"><label class="icon_portion"><img src="../static/3d_img.png" class="images" alt=""></label> </div>
                      <h5>3d promotion</h5>
                      <p class="text_1">3D Animation is a process of creating photorealistic 3D animations that visually depict the configuration</p>
                  </div>
              </b-col>
          </b-row>
           <b-row class="mt-4 content_align">
              <b-col>
                  <div class="service_area">
                      <div class="img_graphic"><label class="icon_portion"><img src="../static/social_img.png" class="images"  alt=""></label> </div>
                      <h5>social media </h5>
                      <p class="text_1">Social media marketing is an online marketing method that utilizes different social media platforms. </p>
                  </div>
              </b-col>
              <b-col>
                   <div class="service_area">
                      <div class="img_graphic"><label class="icon_portion"><img src="../static/invoice_img.png" class="images invoice"  alt=""></label> </div>
                      <h5>invoice call</h5>
                      <p class="text_1">An invoice is a commercial document that itemizes and records a transaction between a buyer and a seller. </p>
                  </div>
              </b-col>
              <b-col>
                   <div class="service_area">
                      <div class="img_graphic"><label class="icon_portion"><img src="../static/map_img.png" class="images" alt=""></label> </div>
                      <h5>google map</h5>
                      <p class="text_1">The Google Maps API is one of those clever of Google technology that helps you take the power of Google Maps.</p>
                  </div>
              </b-col>
          </b-row>

      <!--<img src="https://chart.apis.google.com/chart?cht=qr&chs=250x250&chl=https://alsafartravel.000webhostapp.com/">-->
    </b-container>
    <Footerportion class="mt-4"/>
   

  </div>
</template>

<script>
export default {
    name:'Service_vue',

}
</script>

<style scoped>
*{
    font-family: 'Raleway', sans-serif;
}
.service_back{
  background-image: url("../static/service_banner_img.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  width: 100%;
  height: 500px;
  display: grid;
  place-items: center;
  position: relative;
  color: #fff;
  font-size: 30px;
  text-transform: capitalize;
  margin-top: 10px;
  clip-path: polygon(100% 0, 100% 67%, 93% 97%, 7% 97%, 0 100%, 0% 0%);
}
.service_back::before{
  content: '';
  position: absolute;
  top: 0;
  width: 100%;
  height: 100%;
  background: #1c233f;
  opacity: 0.6;
  transition: 0.5s;
}
.service_back:hover::before{
  width: 60%;
  transition: 0.5s;
}
.text_1{
  position: relative;
  margin: 0;
}
.text_2{
  font-size: 18px;
  margin-top: 10px;
}
.line {
    width: 120px;
    height: 2px;
    background: #f7bc08;
    margin: auto;
    border-radius: 10px;
    position: relative;
}
.line_2 {
    width: 40px;
    height: 5px;
    background: #1c233f;
    margin: auto;
    border-radius: 10px;
    position: relative;
    top: -3px;
}
.service_area{
    background: rgba( 255, 255, 255, 0.25 );
    box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
    backdrop-filter: blur( 4px );
    -webkit-backdrop-filter: blur( 4px );
    border: 1px solid rgba( 255, 255, 255, 0.18 );
    padding: 10px;
    border-top-right-radius: 20px;
    border-bottom-left-radius: 20px;
    transition: 0.5s;                 
} 
.service_area:hover{
    transform: scale(0.9);
}
h5{
    text-transform: capitalize;
    color: #f7bc08;
    text-align: center;
}
.img_graphic, .text_1{
    text-align: center;
}
.icon_portion{
    width: 85px;
    height: 85px;
    background: #1c233f;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 10px auto;
    clip-path: circle(50%)
}
.images{
    width: 59%;
    animation: move 5s infinite;
}
@keyframes move{
    0%{
        transform: translate(-200%);
    }
}
.invoice{
    clip-path: circle(50%);
}
@media screen and (max-width:1200px){
   
    .text_1{
        font-size: 14px;
    }
    .text_p{
        font-size: 28px;
    }
}
@media screen and (max-width:1024px) {
    .text_p{
        font-size: 21px;
    }
    .service_back{
        height: 439px;
    }
}
@media screen and (max-width:992px){
    .text_p{
        display: none;
    }
    .service_back{
        height: 419px;
    }
    .service_back::before{
        background: transparent;
    }
    .text_1{
        font-size: 13px;
    }
    h5{
        font-size: 18px;
    }
}
@media screen and (max-width:768px){
   .text_2{
        font-size: 15px;
   }
   .content_align{
        flex-direction: column;
   }
   .service_area{
        margin: 10px 0px;
   } 
   .service_back{
        height: 336px;
    }
}
@media screen and (max-width:568px){
    .service_back{
        height: 250px;
    }
    .service_area{
        margin: 10px 35px;
    }
    .text_2{
        font-size: 13px;
    } 
}
@media screen and (max-width:480px){
    .service_back{
        height: 200px;
        margin-top: 30px;
    }
    .text_2{
        font-size: 14px;
    }  
}
@media screen and (max-width:360px){
    .service_back{
        height: 180px;
    }
    h3{
        font-size: 25px;
    }
}
</style>