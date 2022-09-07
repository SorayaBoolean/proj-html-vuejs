<template>
  <div>
    <div class="top_header">
      <div class="header_container">
        <div class="call_us">
        <p>
          <i class="fa-solid fa-phone"></i>
           Call us for free at 100.100.100
        </p>
      </div>
      <div class="menu_list">
        <ul>
          <li><i class="fa-brands fa-facebook-f"></i></li> 
          <li><i class="fa-brands fa-twitter"></i></li>
          <li><i class="fa-brands fa-instagram"></i></li>
          <li><i class="fa-brands fa-youtube"></i></li>
        </ul>
      </div>
      </div> 
    </div>


    <div class="bottom_header">
      <div class="header_container">

          <div class="logo_brand">
          <img src="@/assets/img/avada-movers-logo.png" alt="">
        </div>

        <div class="navbar">
          <nav>
            <ul>
              <li v-for="(item,index) in menu" :key="index"><a href="#">{{item}}</a></li> 
              <li><div class="button">Button</div></li>
            </ul>
          </nav>
        </div>
      </div>
    </div>

    <div class="jumbotron">
      <div class="top_jumbotron">
        <div class="jumbotron_text">
          <JumbotronText/>
        </div>
      </div>
      <div class="bottom_jumbotron">
        <h4>
          <i class="fa-regular fa-paper-plane"></i> GET A FREE QUOTE ONLINE NOW!</h4>
      </div>
    </div>
  </div>
    
</template>

<script>
import JumbotronText from './JumbotronText.vue';
export default {
    name: "MyHeader",
    data() {
        return {
            menu: [
                "Home",
                "Rates",
                "Testimonials",
                "FAQ",
                "Blog",
                "Contact"
            ]
        };
    },
    components: { JumbotronText }
}
</script>

<style scoped lang="scss">

  .header_container{
    display: flex;
    justify-content: space-between;
    align-items:center;
    width: 1000px;
    margin: auto;
  }

  .top_header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #69BF14;
    color:white;
    height: 50px;
    width: 100%;
        .menu_list ul{
          display:flex;
          list-style: none;
        }
        li{
          margin: 10px;
        }
  }

  .bottom_header{
    display: flex;
    justify-content: space-around;
    background-color: white;
    height: 80px;
    width: 100%;

      ul {
        display: flex;
      }

      nav ul li {
        list-style: none;
        color: black;
        margin: 20px;
      }
      a {
        color: black;
        text-decoration:none ;
        font-weight: bolder;

            &:hover {
            color:#69BF14;
          }
      }
  }

  .button{
        text-align: center;
        padding: 5px 0px;
        color: #ffffff;
        background-color: #1B74C3;
        height: 30px;
        width: 100px;
        border-radius: 30px;

        &:hover{
          cursor:pointer;
          font-weight: bold;

        }
    }
  
  .button{
    position:absolute;
    top:75px;
  }

  .top_jumbotron{
    height: 500px;
    width: 100%;
    background-image: url(@/assets/img/avada-movers-homeherobackground-final.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    display: flex;
    justify-content: center;
    align-items: center;

  }

  .bottom_jumbotron{
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #1B74C3;
    color:#ffffff;
    height: 90px;
    width:100%;
  }

</style>