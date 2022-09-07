<template>
  <div>
    <div class="top_header">
      <div class="header_container">
        <div class="call_us">
        <p>
          <i class="fa-solid fa-phone"></i>
           call us for free at 100.100.100
        </p>
      </div>
      <div class="menu_list">
        <ul>
          <li>fac</li>
          <li>twi</li>
          <li>you</li>
          <li>ins</li>
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
              <li><a href="#">Home</a></li>
              <li><a href="#">Home</a></li>
              <li><a href="#">Home</a></li>
              <li><a href="#">Home</a></li>
              <li><a href="#">Home</a></li>
              <li><div class="button">Button</div></li>
            </ul>
          </nav>
        </div>
      </div>
    </div>

    <div class="jumbotron">
      <div class="top_jumbotron"></div>
      <div class="bottom_jumbotron"></div>
    </div>
  </div>
    
</template>

<script>
export default {
name: 'MyHeader'
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

  .top_jumbotron{
    height: 400px;
    width: 100%;
    background-image: url(@/assets/img/avada-movers-homeherobackground-final.jpg);
    background-size: contain;
  }

  .bottom_jumbotron{
    background-color: #1B74C3;
    height: 90px;
    width:100%;
  }

</style>