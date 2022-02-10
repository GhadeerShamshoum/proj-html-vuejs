<template>
    <section>    
      <h3>latest news</h3>
      <div class="textContainer">
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur voluptate amet suscipit architecto libero, placeat dolor iusto voluptates voluptatum labore esse voluptatem ea quisquam repellendus aliquid consequatur, error vero alias?</p>
      </div>
      <div class="containerItems">
          <div v-for="(element, index) in lastnews" :key="index" class="card">
              <div class="imageContainer">
                <img :src="require('../../../assets/img/blog/'+element.image+'.jpg') " alt="">
              <div class="hoverCrad">
                <div class="hoverItemsCard">
                  <div class="searchLink">
                    <div class="linki"><i class="linkIcon fa-solid fa-link"></i></div>
                    <div class="searchi"><i class="searchIcon fa-solid fa-magnifying-glass"></i></div>
                  </div>
                  <div class="florida">{{element.title}}</div>
                  <div class="commercial">Architecture, Buildings, Constructions, News</div>
                </div>
              </div>
              </div>
              <div class="textUnderPic">
                <h4 class="title">{{element.title}}</h4>
                <div class="date">{{element.date}}</div>
                <hr>
                <p class="text">{{element.text}}</p>
              </div>
          </div>  
      </div>
      <div class="viewAllPro">View all projects</div>   
  
    </section>
</template>

<script>


export default {
  name: 'LatestNews',
   data(){
      return{
          lastnews:[
              {
                image:"blog-post-134132600",
                title:"Redeveloping Florida's Remote Southern Coast",
                date:"December 7th, 2015",
                text:"Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut faucibus rhoncus sed dignissim leo. Nullam sed metus id sapien Cerca nello screenshot"
              },
              {
                image:"blog-post-92486644",
                title:"How We Manage Large Construction Projects",
                date:"December 7th, 2015",
                text:"Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut faucibus rhoncus sed dignissim leo. Nullam sed metus id sapien Cerca nello screensho"
              }, 
              {
                image:"blog-post-332773904",
                title:"Future proofing a modern home",
                date:"December 7th, 2015",
                text:"Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut faucibus rhoncus sed dignissim leo. Nullam sed metus id sapien Cerca nello screensho"
              },   
          ]
      }
  },
  
 

  
  props: {
    
  },

}
</script>


<style scoped lang="scss">
@import "../../../assets/style/variabiles.scss";
section{
  background-color: #eeeded;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
h3{
  font-weight: 300;
  text-transform: capitalize;
  position: relative;
  padding: 20px 0;
  &::after{
    content: "";
    border-bottom: 2px solid $brightSun;
    position: absolute;
    bottom: 0;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 130px;
  }
}

.textContainer{
  width: 850px;
  p{
    margin: 50px 0;
    font-weight: 100px;
    color: $doveGray;
  }
}
.containerItems{
    width: 1000px;
    display: flex;
    .card{
        width: calc(100% / 3 - 20px);
        margin: 0 10px;
        position: relative;
        &:hover .hoverCrad{
          display: block;
          transition: all .8s linear;
        }
         .hoverCrad{
            position: absolute;
            top:0;
            right: 0;
            width: 100%;
            height: 200px;
            background-color: $brightSun;
            display: none;
            .hoverItemsCard{
              height: 100%;
              padding: 40px;
              display: flex;
              flex-direction: column;
              justify-content: center;
              align-items: center;
              .searchLink{
                display: flex;
                .searchi,
                .linki{
                  height: 50px;
                  width: 50px;
                  background-color: white;
                  border-radius: 50%;
                  margin: 10px;
                  display: flex;
                  justify-content: center;
                  align-items: center;
                  .searchIcon,
                  .linkIcon{
                    color: $sun;
                  }
          
          }
        }
        .florida{
          font-size: 15px;
          color:white;
          text-align: center;
        }
        .commercial{
          font-size: 10px;
          text-align: center;
          color:white;
          margin: auto;
        }
              }
        }
        .imageContainer{
            width: 100%;
            height: 200px;
           
            img{
                width: 100%;
            }
        }
        .textUnderPic{
            padding: 20px;
            .title{
                font-size: 22px;
                font-weight: 400;
            }
            .date{
                font-size: 10px;
            }
            .text{
                font-size: 15px;
            }
            .title,
            .date,
            .text{
                color:$doveGray;
            }
            hr{
                width: 100%;
            }
        }

    }
}
.viewAllPro{
  position: relative;
  text-transform: uppercase;
  color:$doveGray;
  letter-spacing: 0.1rem;
  font-size: 15px;
  margin:60px 0;
}

.viewAllPro::before{
  content: '';
  position: absolute;
  left: 188px;
  top:50%;
  width: 393px;
  border: 2px solid $white;
}
.viewAllPro::after{
  content: '';
  position: absolute;
  right: 188px;
  top:50%;
  width: 393px;
  border: 2px solid $white;
}


</style>
