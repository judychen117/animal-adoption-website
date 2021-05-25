<template>
  <div>
    <Navbar />
    <div class="container top-position">
      <p class="navbar-brand">胖達</p>
      <div class="dog-profile-wrapper">
        <div class="border main-content">
          <div class="card-content">
            <i class="fas fa-venus-mars fa-4x"></i>
            <p class="card-description">男孩</p>
          </div>
          <div class="card-content">
            <i class="fas fa-baby-carriage fa-4x"></i>
            <p class="card-description">青少年</p>
          </div>
          <div class="card-content">
            <i class="fas fa-palette fa-4x"></i>
            <p class="card-description">白底、黑班</p>
          </div>
          <div class="card-content">
            <i class="fas fa-home fa-4x"></i>
            <p class="card-description">中型犬</p>
          </div>
          <div class="card-content">
            <i class="far fa-smile fa-4x"></i>
            <p class="card-description">溫和、慢熟</p>
          </div>
        </div>
        <div class="border sm-pic-left card">
          <img
            src="./../assets/dog-panda2.jpg"
            alt="sub-photo"
            class="photo-sub card-img"
          />
          <div class="card-text">
            <p class="card-description">
              胖達聰明又膽小，矛盾的心理萌到讓大家不要不要的 ----志工 曉晴
            </p>
          </div>
        </div>
        <div class="border sm-pic-middle card">
          <img
            src="./../assets/dog-panda3.jpg"
            alt="sub-photo"
            class="photo-sub card-img"
          />
          <div class="card-text">
            <p class="card-description">
              喜歡遠離人群、在動物之家免強交到的唯一朋友就是他室友 ----志工 曉晴
            </p>
          </div>
        </div>
        <div class="border sm-pic-right card">
          <img
            src="./../assets/dog-panda4.jpg"
            alt="sub-photo"
            class="photo-sub card-img"
          />
          <div class="card-text">
            <p class="card-description">
              經驗告訴我只要他喜歡你就會在你出現時一直亂叫、討摸 ----志工 曉晴
            </p>
          </div>
        </div>
        <div class="border big-pic">
          <video
            class="photo-main"
            controls
            src="./../assets/dog-panda-video.mp4"
          ></video>
        </div>
      </div>
      <br />
      <br />
      <br />
      <br />
      <br />
      <p class="navbar-brand">阿Ｑ</p>
      <div class="dog-profile-wrapper2">
        <div class="border main-content">
          <div class="card-content">
            <i class="fas fa-venus-mars fa-4x"></i>
            <p class="card-description">女孩</p>
          </div>
          <div class="card-content">
            <i class="fas fa-baby-carriage fa-4x"></i>
            <p class="card-description">中年</p>
          </div>
          <div class="card-content">
            <i class="fas fa-palette fa-4x"></i>
            <p class="card-description">全黑</p>
          </div>
          <div class="card-content">
            <i class="fas fa-home fa-4x"></i>
            <p class="card-description">中型犬</p>
          </div>
          <div class="card-content">
            <i class="far fa-smile fa-4x"></i>
            <p class="card-description">害羞、聰明</p>
          </div>
        </div>
        <div class="border sm-pic-left card">
          <img
            src="./../assets/dog-Q1.jpg"
            alt="sub-photo"
            class="photo-sub card-img"
          />
          <div class="card-text">
            <p class="card-description">
              由於以前待過成犬社，每次只要經過成犬社她都想回去，是個迷戀舊家的忠心狗狗
              ----志工 曉晴
            </p>
          </div>
        </div>
        <div class="border sm-pic-middle card">
          <img
            src="./../assets/dog-Q2.jpg"
            alt="sub-photo"
            class="photo-sub card-img"
          />
          <div class="card-text">
            <p class="card-description">
              屬於守舊派狗狗，堅持己見的新時代女性 ----志工 曉晴
            </p>
          </div>
        </div>
        <div class="border sm-pic-right card">
          <img
            src="./../assets/dog-Q2.jpg"
            alt="sub-photo"
            class="photo-sub card-img"
          />
          <div class="card-text">
            <p class="card-description">有時候害羞到有點三八 ----志工 曉晴</p>
          </div>
        </div>
        <div class="border big-pic">
          <video
            class="photo-main"
            controls
            src="./../assets/dog-Q-video.mp4"
          ></video>
        </div>
      </div>
      <br />
      <br />
      <br />
      <br />
      <br />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "./../components/Navbar.vue";

export default {
  name: "Main",
  components: {
    Navbar,
  },
};
</script>

<style scoped>
.container {
  padding-top: 140px;
  height: 100%;
}
.dog-profile-wrapper {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  grid-template-rows: repeat(2, 220px);
  grid-gap: 1rem;
  grid-template-areas:
    "main main main big big"
    "left middle right big big";
}
.border {
  border-radius: 20px;
}
.card-content {
  display: block;
  padding-right: 30px;
  text-align: center;
}
.card-content i {
  padding-bottom: 10px;
}
.main-content {
  grid-area: main;
  display: flex;
  justify-content: center;
  align-items: center;
}
.photo-main {
  width: 100%;
  height: 460px;
  display: block;
  object-fit: cover;
  border-radius: 20px;
}
.photo-sub {
  width: 100%;
  height: 220px;
  display: block;
  object-fit: cover;
  border-radius: 20px;
}
.sm-pic-left {
  grid-area: left;
}
.sm-pic-middle {
  grid-area: middle;
}
.sm-pic-right {
  grid-area: right;
}
.big-pic {
  grid-area: big;
}
.dog-profile-wrapper2 {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  grid-template-rows: repeat(2, 220px);
  grid-gap: 1rem;
  grid-template-areas:
    "big big main main main"
    "big big left middle right ";
}
</style>
