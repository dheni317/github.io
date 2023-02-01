<template>
  <div class="profile_container">
    <h1 class="title">Profile</h1>
    <img class="kuromii" src="../img/kuromi1.png" alt="kuromii" />
    <img class="profile_img" src="../img/killerwhale.jpg " alt="killerwhale" />
    <img class="kuromii" src="../img/kuromi1.png" alt="kuromii" />
    <h4 class="profile_name">황동현(kind_killerwhale)</h4>
    <p class="profile_intro">
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Repudiandae
      accusamus voluptates, enim magni maxime odio perspiciatis commodi suscipit
      non iusto ipsa sunt quibusdam vitae corrupti facilis cupiditate
      repellendus nobis veniam.
    </p>
    <img class="sns_img" src="../img/instagram.png" alt="instagram" @click="GoToLink('https://instagram.com/mad_killerwhale')"/>
    <div class="line"></div>
    <img class="sns_img" src="../img/github.png" alt="github" @click="GoToLink('https://github.com/dheni317')" />
    <div class="line"></div>
    <img class="sns_img" src="../img/mail.png" alt="mail" @click="GoToLink('mailto:hdh317817@gmail.com')"/>
    <hr />
  </div>
</template>

<script>
export default {
  name: "ProfileComponent",
  methods:{
    GoToLink(url){
      window.open(url);
    },
  }
};
</script>

<style>
.profile_container {
  text-align: center;
  width: 90%;
  margin: 0 5%;
}

.title {
  font-size: 45px;
  font-family: "ccsignlanguage", "sans-serif";
  margin: 18px 0 7px 0;
}

.profile_img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  border: solid #707070 1px;
  margin: 13px 25px;
}

.kuromii {
  width: 200px;
  height: 200px;
}

.profile_name {
  font-size: 23px;
  margin: 10px 0 15px 0;
  font-family: "NanumSquareRound";
}

.profile_intro {
  font-size: 15px;
  max-width: 60%;
  margin: 0 20% 17px 20%;
  font-family: "NanumBarunPen";
}

.line {
  display: inline-block;
  width: 2px;
  height: 30px;
  background-color: black;
  margin: 0 5px;
}

.sns_img {
  width: 30px;
  height: 30px;
}

hr {
  width: 90%;
  margin-top: 10px;
}
</style>