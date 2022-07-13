<template>
<div class="contactportion">
    <b-container>
        <div class="form_portion">
            <h3 class="text-center text-capitalize">Get in touch</h3>
            <div class="row mt-5">
                <div class="col-lg-6 left_form">
                    <div class="row callus_portion">
                        <div class="col-lg-2">
                            <div class="icon_back"><i class="fa fa-phone" aria-hidden="true"></i></div>
                        </div>
                        <div class="col-lg-10">
                            <p class="text_1 mb-0 text-uppercase">call us</p><strong class="call_num"><a href="tel:9111170884">+91 91111-70884</a></strong>
                        </div>
                    </div>
                    <div class="row mt-5 envelope_portion">
                        <div class="col-lg-2">
                            <div class="icon_back"><i class="fa fa-envelope" aria-hidden="true"></i></div>
                        </div>
                        <div class="col-lg-10">
                            <p class="text_1 m-0 text-uppercase">mail us</p><strong class="email"><a href="mailto:shantanu@smdigitaltech.com">shantanu@smdigitaltech.com</a></strong>
                        </div>
                    </div>
                </div>
                <div class="or_section">OR</div>
                <div class="col-lg adjust">
                    <form id="myForm" action="https://script.google.com/macros/s/AKfycbzoBMZk8rTFHhABOyWBUJXYkfAjctHvr0YJ_BiaeGKzOpRDM7NNUtHzJnf0UjRQudIGZw/exec"  method="post">
                        <div class=" form_input_portion">
                            <input type="text" class="mb-4 p-2" name="Name" maxlength="40" v-model="user.name" required>
                            <label>Name</label>
                        </div>
                        <div class="form_input_portion">
                            <input type="tel" class="mb-4 p-2" name="Number" maxlength="10" v-model="user.number" required>
                            <label>Number</label>
                        </div>
                        <div class=" form_input_portion">
                            <input type="email" class="mb-3 p-2" name="Email" v-model="user.email" required>
                            <label>Email</label>
                        </div>
                        <div class="button_section">
                            <button type="submit" class="mt-1 py-2 px-4 text-uppercase login" @submit="LoginForm"  @click="FormLogin">login</button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </b-container>

</div>
</template>

<script>
//import axios from 'axios'
export default {
    name: 'Contactportion',

    data() {
        return {
            user: {
                name: '',
                number: '',
                email: ''
            }
        }
    },
    methods: {
        LoginForm() {
            if(this.user.name == '' || this.user.number == '' || this.user.email == '' ){
                alert('please input this field!')
            }
        },
        FormLogin(){
            if(this.user.name == '' || this.user.number == '' || this.user.email == '' ){
                alert('Please input this field!')
            }else{
                alert('Thank You!');
            }
            
        }
        

       
    }
}
</script>

<style scoped>
.contactportion {
    width: 100%;
    height: auto;
    display: grid;
    place-items: center;
    background: url(../static/contact_img.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    box-sizing: border-box;
    padding: 30px 0px;
    background-attachment: fixed;
}

.form_portion {
    width: 70%;
    height: 350px;
    background: rgba(255, 255, 255, 0.8);
    box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
    backdrop-filter: blur(4px);
    border-radius: 10px;
    border: 1px solid rgba(255, 255, 255, 0.18);
    position: relative;
    margin: auto;
    padding: 20px;
}

.icon_back {
    width: 40px;
    height: 40px;
    background: transparent;
    border-radius: 50%;
    border: 1px solid #fff;
    display: grid;
    place-items: center;
    box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.5);
}

.call_num,
.email {
    font-size: 17px;

}

.call_num>a,
.email>a {
    color: #1c233f;
}

.left_form {
    border-right: 1px solid #c7c8ca;
    padding: 0px 18px !important;
}

.callus_portion,
.envelope_portion {
    align-items: center;
}

.text_1 {
    font-weight: 500;
    color: #000;
}

.or_section {
    width: 34px;
    height: 34px;
    background: #edf2f5;
    border-radius: 50%;
    border: 1px solid #fff;
    position: relative;
    top: 74px;
    left: -17px;
    display: grid;
    place-items: center;
    box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.5);
}

input {
    width: 100%;
    margin: auto;
    border: 1px solid #929292;
    border-radius: 5px;
    background: transparent;
    outline: none;
    color: #1c233f;
    font-weight: 500;
}

.form_input_portion {
    position: relative;
}

.form_input_portion>label {
    position: absolute;
    left: 9px;
    top: 14%;
}

.form_input_portion input:valid~label,
.form_input_portion input:focus~label {
    color: #fff;
    transform: translateX(2px) translateY(-30px);
    transition: 0.3s;
    background: #1c233f;
    border-radius: 2px;
    padding: 0px 8px;
}

::placeholder {
    color: #000;
    text-transform: capitalize;
}

.login {
    background: #1c233f;
    border: none;
    color: #fff;
    border-radius: 5px;
    letter-spacing: 5px;
}

.login:hover {
    background: #f6bb00;
    color: #1c233f;
}

h3 {
    color: #1c233f;
}

.button_section {
    width: 100%;
    display: flex;
    justify-content: center;
}

@media screen and (max-width:1024px) {
    input {
        width: 90%;
    }
}

@media screen and (max-width:992px) {
    .form_portion {
        height: auto;
    }

    input {
        width: 70%;
    }

    .form_input_portion {
        text-align: center;
    }

    .form_input_portion>label {
        left: 75px;
        top: 15%;
    }

    .callus_portion,
    .envelope_portion {
        text-align: center;
    }

    .icon_back {
        margin: 10px auto;
    }

    .left_form {
        border: none;
    }

    .or_section {
        visibility: hidden;
    }
}

@media screen and (max-width:768px) {
    input {
        width: 80%;
    }

    .form_input_portion>label {
        left: 50px;
    }

    .form_portion {
        width: 90%;
    }
}

@media screen and (max-width:480px) {
    .form_input_portion>label {
        left: 42px;
    }
}

@media screen and (max-width:360px) {
    .form_input_portion>label {
        left: 20px;
    }

    input {
        width: 90%;
    }

    .email>a {
        font-size: 15px;
    }
}
</style>
