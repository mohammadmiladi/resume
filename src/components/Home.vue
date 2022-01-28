<template>
  <div class="main-style">
    <b-container>
      <b-row>
        <b-col lg="3">
          <div class="left-side">
            <div class="blue-block"></div>
            <div class="bio-block">
              <div class="name-style">MOHAMMAD</div>
              <div class="name-style">MILADI</div>
              <img
                class="image-style"
                src="@/assets/mohammad.jpg"
                alt="mohammad"
              />
              <div class="bio-section">
                <div>Date of birth : 1993 - 06 - May</div>
                <div>Gender : Men</div>
                <div>Location-Region : Tehran</div>
                <div>Work Exprience : 9 years</div>
                <div>Military Service Status : Exemption during education</div>
              </div>
            </div>
          </div>
        </b-col>
        <b-col lg="9">
          <div class="right-side">
            <div class="right-title">
              <div>My Story</div>
              <div class="right-underline"></div>
            </div>
            <div>
              <div class="my-story">
                I have been working in the IT industry for about 9years. I have
                worked for 2years as a project control expert, 5years as a
                digital marketing expert and manager, and for the last 2years as
                a front-end programmer.
              </div>
              <div class="my-story">
                During these 2years that I worked as a front-end programmer, I
                participated in 7 different projects. worked on different
                technologies, my interest in programming increased day by day.
              </div>
            </div>
             <div class="right-title">
              <div>My Soft Skills</div>
              <div class="right-underline"></div>
            </div>
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.main-style {
  padding: 80px 50px;
  min-height: 100vh;
  height: 100%;
  background-color: rgb(222, 232, 238);
}
.left-side {
  box-shadow: 0px 40px 64px -12px rgba(0, 0, 0, 0.08),
    0px 0px 14px -4px rgba(0, 0, 0, 0.05), 0px 32px 48px -8px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
  padding: 25px 0;
  background-color: white;
  min-height: 550px;
}
.right-side {
  box-shadow: 0px 40px 64px -12px rgba(0, 0, 0, 0.08),
    0px 0px 14px -4px rgba(0, 0, 0, 0.05), 0px 32px 48px -8px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
  padding: 25px;
  background-color: white;
  min-height: 550px;
}
.blue-block {
  background-color: rgb(130 72 252);
  width: 85%;
  height: 35px;
}
.bio-block {
  padding: 25px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.name-style {
  font-weight: 700;
  font-size: 30px;
  color: rgb(56 0 174);
}
.image-style {
  margin-top: 20px;
  border-radius: 30px;
  width: 100%;
}
.bio-section {
  font-weight: 700;
  margin-top: 20px;
  display: flex;
  flex-direction: column;
  font-size: 14px;
}
.right-title {
  font-size: 20px;
  margin-bottom: 20px;
  margin-top: 20px;
  font-weight: 700;
  color: rgb(56 0 174);
}
.right-underline {
  width: 90%;
  height: 2px;
  margin-top: 5px;
  background-color: rgb(130 72 252);
}
.my-story {
  font-size: 16px;
  line-height: 26px;
  text-align: justify;
}
</style>
