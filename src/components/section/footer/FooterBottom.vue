<template>
<footer class="bottomContainer">
  <div class="container">
    <div class="item">
      <img class="logoFooter" src="../../../assets/img/footer/footer-logo.png" alt="">
      <p>exclusive properties Our work inspires We pride We are specialists in the construction of unique and ourselves on delivering outstanding quality and design for leading clients across the world</p>
      <button class="buttonFooterTop"><a href="#">Learn More</a></button>
    </div>
    <div class="item">
      <h6>Latest tweets</h6>
      <div class="tweetUser">
        <div class="smallIconContainer">
          <img class="profilePic" src="../../../assets/img/footer/3a74ce3d0532b7773b174c45ca3bd05a_normal.png" alt="">
        </div>
        <div class="userName">
          <div class="nameTagContainer">
            <div class="name">ThemeFusion</div>
            <div class="tag">@Theme_Fusion</div>
          </div>
          <div class="tweeter">
            <img class="iconTweeter" src="../../../assets/img/footer/image (1).svg" alt="">
          </div>
          <p class="textTweet">Do you need sublime WordPress hosting for your next website? Take advantage of exclusive partner offers that we have secured just for you, &#38; launch your site in seconds with <span>#avada</span>  on WP Engine hosting &#38; get 30% Off this Black Friday <span>bil.ly/kLLE2 #BackFriday2020</span></p>
          <div class="adImg"><img src="../../../assets/img/footer/En2TRxLW4AEiWUN.jpeg" alt=""></div>
          <div class="containerIconsB">
            <div>
              <span><img class="iconBottom" src="../../../assets/img/footer/image (2).svg" alt=""></span>
              <span><img class="iconBottom" src="../../../assets/img/footer/image (3).svg" alt=""></span>
              <i class="fa-solid fa-up-right-from-square"></i>
            </div>
            <div class="hours">22h</div>
          </div>
        </div>
      </div>
    </div>
    <div class="item">
      <h6>contact us today</h6>
      <ul v-for="(element,index) in list" :key="index">
        <li class="listItems">
          <div class="iconList"><i :class=(element.icon)></i></div>
          <div class="textList">
            <div>{{element.li}}</div>
            <div>{{element.li2}}</div>
            <div> {{element.li3}}</div>
          </div>
        </li>
      </ul>
    </div>
    <div class="findUs">
      <h6>Find Us</h6>
    </div>
  </div>  
</footer>
 
</template>

<script>
export default {
  name: 'FooterBottom',
  data(){
    return{
      list:[
        {
          icon:"fa-solid fa-globe",
          li:"Corporate Location",
          li2:"1600 Amphitheatre Parkway",
          li3:"London WC11BA"
        },
        {
          icon:"fa-solid fa-house-chimney",
          li:"Residential Location",
          li2:"9521 Broadsberry Avenue",
          li3:"Paddington RC7 9ZA"
        },
        {
          icon:"fa-solid fa-phone-flip",
          li:"1.800.458556/1.8005322112",
        },
        {
          icon:"fa-solid fa-envelope",
          li:" info@your-domain.com",
        },
        {
          icon:"fa-solid fa-clock",
          li:"Monday-Friday: 9:00 AM-6:00 PM",
        },
        {
          icon:"fa-solid fa-clock",
          li:"Saturday Sunday: 9:00 AM-12:00 PM",
        },
      ]

    }
  },

    
  props: {
    
  }
}
</script>


<style scoped lang="scss">
@import "../../../assets/style/variabiles.scss";
.bottomContainer{
  height: 545px;
  background-color: $codGray;
  display: flex;
  align-items: center;
  .item{
    width: calc(100% / 4 - 40px);
    margin: 0 20px;
    .logoFooter{
      height: 59px;
    }
    p{
      color: $doveGray;
      line-height: 28px;
      font-size: 13px;
      padding: 30px 0;
    }

  }
 
}
.buttonFooterTop{
    position: relative;
    border: none;
    padding: 11px 40px;
    background-color: $brightSun;
    a{
      letter-spacing: 0.1rem;
      color:$doveGray ;
    }
  }
h6{
  color: $sun;
  font-weight: 900;
  font-size: 15px;
  letter-spacing: 0.1rem;
  text-transform: uppercase;
  margin-bottom: 32px;
}
.smallIconContainer{
  height: 100%;
  width: 15%;
  .profilePic{
    width: 100%;
    border-radius: 50%;
    padding: 0 3px;
  }
}
.tweetUser{
  display: flex;
  .userName{
    padding: 5px;
    width: 85%;
    position: relative;
    .tweeter{
      position: absolute;
      top:0;
      right: 0;
      height: 20px;
      width: 20px;
      .iconTweeter{
        width: 100%;
      }
    }
    .nameTagContainer{
      width: 100%;
      .name{
        color: $white;
        font-size: 14px;
        font-weight: 700;
      }
      .tag{
        color: $LimedSpruce;
        font-size: 10px;
      }
      }
      .textTweet{
        line-height: 15px;
        font-weight: 500;
        color: $white;
      }
      span{
        color: #045287;
      }
      .adImg{
        width: 100%;
        img{
          width: 100%;
        }
      }
      .containerIconsB{
        display: flex;
        justify-content: space-between;
        .iconBottom{
          width: 10px;
          margin-left: 10px;
        }
        .hours{
          color: $LimedSpruce;
          font-size: 10px;
        }
      }
    }
  }
.listItems{
  display: flex;
  
  .iconList{
    color:  $doveGray;
    margin-right: 12px;
  }
  .textList{
    color:  $doveGray;
    font-size: 13px;

  }
}

</style>
