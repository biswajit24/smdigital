<template>
  <div class="contact">
    <Navbarportion />
    <div class="contact_banner">
      <b-container>
            <h2 class="text-capitalize">contact us</h2>
            <div class="text-capitalize text_1"></div>
      </b-container>
    </div>
    <b-container>
      <b-row class="mt-5 img_align">
        <b-col>
          <div class="left_contact">
            <div class="address">
              <img src="../static/location.png" class="flat_icon" alt="">
            </div>
            <p class="text_2 text-capitalize"><a href="https://goo.gl/maps/NfV4U5b1qMwvBMcp6" target="_blank">garia, kolkata, india</a></p>
          </div>
          <div class="left_contact">
            <div class="address">
              <img src="../static/call.png" class="flat_icon" alt="">
            </div>
            <p class="text_2"><a href="tel:9111170884">9111170884 /</a> <a href="tel:7000375881">7000375881</a> </p>
          </div>
          <div class="left_contact">
            <div class="address">
              <img src="../static/envelope.png" class="flat_icon" alt="">
            </div>
            <p class="text_2"><a href="mailto:shantanu@smdigitaltech.com">shantanu@smdigitaltech.com</a></p>
          </div>
        </b-col>
        <b-col class="right_img"><img src="../static/contact_img.png" alt=""></b-col>
      </b-row>
    </b-container>
     
    <div class="map">
      <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3687.0919684674013!2d88.3795444!3d22.463178!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3a0271a17947327f%3A0x57250cb2d3be2d3c!2sTribeni%20Apartment%2C%20Garia%20Main%20Rd%2C%20Purbapara%2C%20Kamdahari%2C%20Kolkata%2C%20West%20Bengal%20700084!5e0!3m2!1sen!2sin!4v1656483541756!5m2!1sen!2sin" width="100%" height="600" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
    </div>
    <Footerportion />
  </div>
</template>

<script>
export default {
  name:'Contact_vue',

}
</script>

<style scoped>
  .contact_banner{
    width: 100%;
    height: 450px;
    background: url("../static/contactpage_img.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    display: flex;
    align-items: center;
    position: relative;
    clip-path: polygon(100% 0, 100% 67%, 93% 97%, 7% 97%, 0 100%, 0% 0%);
  }
  .contact_banner::before{
  content: '';
  position: absolute;
  top: 0;
  width: 100%;
  height: 100%;
  background: #1c233f;
  opacity: 0.6;
  }
  .text_1{
    width: 80px;
    height: 5px;
    background: #f7bc08;
    position: relative;
    border-radius: 10px;

  }
  h2{
    position: relative;
    color: #fff;
    font-size: 40px;
  }
  .right_img{
    display: flex;
    justify-content: flex-end;
  }
  .left_contact{
    background: #1c233f;
    width: 50%;
    text-align: center;
    padding: 15px 5px;
    margin-bottom: 10px;
  }
  .left_contact:hover{
    cursor: pointer;
  }
  .left_contact:nth-child(1), .left_contact:nth-child(2), .left_contact:nth-child(3){
    transition: all 0.6s ease-in-out;
    transform: translateX(0px);
  }
  .left_contact:nth-child(1):hover{
    transform: translateX(30px);
  }
  .left_contact:nth-child(2):hover{
    transform: translateX(30px);
  }
  .left_contact:nth-child(3):hover{
    transform: translateX(30px);
  }
  .address{
    background: #f7bc08;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: auto;
  }
  .text_2{
    margin-top: 10px;
  }
  .text_2 > a{
    color: #fff;
    text-decoration: none;
  }
  .text_2 > a:hover{
    color: #f7bc08;
  }
  .icons{
    font-size: 19px;
    color: #1c233f;
  }
  .map{
    width: 100%;
    margin-top: 20px;
    position: relative;
    top: 5px;
  }

  @media screen and (max-width:992px){
    .right_img > img{
      width: 88%;
      object-fit: scale-down;
    }
    .left_contact{
      width: 80%;
    }
    .img_align{
      align-items: center;
    }
    h2{
      color: #f7bc08;
    }
    .text_1{
      background: #ccc;
    }
  }
  @media screen and (max-width:768px){
    .img_align{
      flex-direction: column;
    }
    .left_contact{
      margin: 10px auto;
    }
    .right_img{
      justify-content: center;
    }
  }
  @media screen and (max-width:568px){
     h2{
      font-size: 35px;
    }
  }
  @media screen and (max-width:480px){
    .right_img > img{
      width: 60%;
    }
  }
   @media screen and (max-width:360px){
   
  }
</style>