<template>
  <div class="service_portion">
    <h3 class="text-center text-uppercase service pt-5">our services</h3>
    <div class="line"></div>
    <div class="line_2"></div>
    <div class="service_back">
      <b-container>
          <b-row class="mt-5 query">
              <b-col>
                  <div class="service_area">
                      <div class="img_graphic"><label class="icon_portion"><img src="../static/marketing_img.png" class="images"  alt=""></label> </div>
                      <h5>branding marketing</h5>
                      <p class="text_1">Brand marketing is promoting a brand's products or services in a way that elevates the brand as a whole. It involves creating and maintaining brand-consumer relationships and marketing brand attributes.</p>
                  </div>
              </b-col>
              <b-col>
                   <div class="service_area">
                      <div class="img_graphic"><label class="icon_portion"><img src="../static/graphic_design.png" class="images"  alt=""></label> </div>
                      <h5>Graphic design</h5>
                      <p class="text_1">2D Design is the most common technique used for the animated videos (e.g. educational videos, explainer videos, animated commercials, animated films, etc) we produce at our studio.</p>
                  </div>
              </b-col>
              <b-col>
                   <div class="service_area">
                      <div class="img_graphic"><label class="icon_portion"><img src="../static/web_img.png" class="images"  alt=""></label> </div>
                      <h5>web design & seo</h5>
                      <p class="text_1">
                        It provides you with a customized website design that's perfect for your business or personal site.It can mean working on a brand new website or updating an already existing site.
                      </p>
                  </div>
              </b-col>
          </b-row>
          <b-row class="mt-4 query">
              <b-col>
                  <div class="service_area">
                      <div class="img_graphic"><label class="icon_portion"><img src="../static/bulk_img.png" class="images"  alt=""></label> </div>
                      <h5>bulk sms </h5>
                      <p class="text_1">It refers to businesses sending SMS to one or more recipients via bulk SMS service providers such as Textlocal. It is the dissemination of large numbers of SMS messages for delivery to mobile phone terminals. </p>
                  </div>
              </b-col>
              <b-col>
                   <div class="service_area">
                      <div class="img_graphic"><label class="icon_portion"><img src="../static/app_img.png" class="images"  alt=""></label> </div>
                      <h5>mobile app</h5>
                      <p class="text_1">A Mobile app is a software application developed specifically for use on small, wireless computing devices, such as smartphones and tablets, rather than desktop or laptop computers.</p>
                  </div>
              </b-col>
              <b-col>
                   <div class="service_area">
                      <div class="img_graphic"><label class="icon_portion"><img src="../static/3d_img.png" class="images" alt=""></label> </div>
                      <h5>3d promotion</h5>
                      <p class="text_1">
                        3D Animation is a process of creating photorealistic 3D animations that visually depict the configuration, assembly, and inner-workings of a product in the form of an animated video.
                      </p>
                  </div>
              </b-col>
          </b-row>
      </b-container>
    </div>

  </div>
</template>

<script>
export default {
    name:'Service_vue',

}
</script>

<style scoped>

    .service{
        font-weight: 700;
        color: #1c233f;
        font-size: 32px;
        opacity: 0.8;
        letter-spacing: 5px;
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
    }
    .service_area:hover{
        background: #1c233f;
    }
    h5{
        color: #f7bc08;
        text-transform: uppercase;
    }
    h4,.icon_portion{
        color: #fff;
    }
    .text_1{
        font-size: 15px;
        color: #fff;
    }
    .service_back{
        background: #1c233f;
        padding: 40px 0px;
        clip-path: polygon(92% 7%, 100% 2%, 100% 100%, 0 100%, 0 40%, 7% 8%)
    }
    .line{
        width: 120px;
        height: 2px;
        background: #f7bc08;
        margin: auto;
        border-radius: 10px;
    }
    .line_2{
        width: 40px;
        height: 5px;
        background: #1c233f;
        margin: auto;
        border-radius: 10px;
        position: relative;
        top: -4px;
    }
    .fa-mobile{
        font-size: 30px;
    }
    .img_graphic{
        position: relative;
        top: -20px;
    }
    .icon_portion{
        width: 80px;
        height: 80px;
        background: rgba( 255, 255, 255, 0.18 );
        border-top-left-radius: 15px;
        border-bottom-right-radius: 15px;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .images{
        width: 58%;
    }

    @media screen and (max-width:1024px){
        .service{
            font-size: 27px;
        }
        .line_2{
            height: 4px;
            top: -3px;
        }
        .query{
            flex-direction: column;
            width: 88%;
            margin: auto;
        }
        .service_area{
            margin: 10px 0px;
        }
        .service_back{
            clip-path: polygon(92% 5%, 100% 2%, 100% 100%, 0 100%, 0 10%, 7% 5%);
        }
    }
    @media screen and (max-width:992px){
        .service_area{
            margin: 15px 0px;
        }
    }
    @media screen and (max-width:600px){
        .service{
            font-size: 23px;
        }
        .line_2{
            height: 4px;
            top: -3px;
        }
        h5{
            font-size: 19px;
        }
        .text_1{
            font-size: 14px;
        }
    }
    @media screen and (max-width:480px){
        .service_back{
        clip-path: polygon(92% 4%, 100% 2%, 100% 100%, 0 100%, 0 10%, 7% 4%);
    }
    }
    @media screen and (max-width:360px){
        .query{
            width: 100%;
        }
    }
</style>