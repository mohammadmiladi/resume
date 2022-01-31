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
                <div class="mt-3">EDUCATION:</div>
                <div>
                  2018 – Present: Strategic Management - Master's degree
                </div>
                <div>
                  2011 – 2017: Industrial Engineering - Bachelor's degree
                </div>
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
            <div>
              <b-row class="w-100 mb-3" style="justify-content: space-between">
                <b-col lg="3" class="soft-skill">Project management</b-col>
                <b-col lg="3" class="soft-skill">Strong decision maker</b-col>
                <b-col lg="3" class="soft-skill">Complex problem solver</b-col>
              </b-row>
              <b-row class="w-100" style="justify-content: space-between">
                <b-col lg="3" class="soft-skill">Teamwork</b-col>
                <b-col lg="3" class="soft-skill">Fast Learner</b-col>
                <b-col lg="3" class="soft-skill">Motivated</b-col>
              </b-row>
            </div>
            <div class="right-title">
              <div>My Programming Skills</div>
              <div class="right-underline"></div>
            </div>
            <b-row class="w-100 mb-3" style="justify-content: space-between">
              <b-col lg="3" class="d-flex align-items-center skill-name">
                <div>HTML</div>
                <div><Stars :rate="85" /></div>
              </b-col>
              <b-col lg="3" class="d-flex align-items-center skill-name">
                <div>CSS</div>
                <div><Stars :rate="85" /></div>
              </b-col>
              <b-col lg="3" class="d-flex align-items-center skill-name">
                <div>JAVASCRIPT</div>
                <div><Stars :rate="75" /></div>
              </b-col>
            </b-row>
            <b-row class="w-100 mb-3" style="justify-content: space-between">
              <b-col lg="3" class="d-flex align-items-center skill-name">
                <div>Vue.js</div>
                <div><Stars :rate="85" /></div>
              </b-col>
              <b-col lg="3" class="d-flex align-items-center skill-name">
                <div>Nuxt.js</div>
                <div><Stars :rate="70" /></div>
              </b-col>
              <b-col lg="3" class="d-flex align-items-center skill-name">
                <div>VueX</div>
                <div><Stars :rate="70" /></div>
              </b-col>
            </b-row>
            <b-row class="w-100 mb-3" style="justify-content: space-between">
              <b-col lg="3" class="d-flex align-items-center skill-name">
                <div>Bootstrap</div>
                <div><Stars :rate="80" /></div>
              </b-col>
              <b-col lg="3" class="d-flex align-items-center skill-name">
                <div>Git</div>
                <div><Stars :rate="60" /></div>
              </b-col>
              <b-col lg="3" class="d-flex align-items-center skill-name">
                <div>Jira</div>
                <div><Stars :rate="60" /></div>
              </b-col>
            </b-row>
            <b-row class="w-100" style="justify-content: space-between">
              <b-col lg="3" class="d-flex align-items-center skill-name">
                <div>React</div>
                <div><Stars :rate="50" /></div>
              </b-col>
              <b-col lg="3" class="d-flex align-items-center skill-name">
                <div>Redux</div>
                <div><Stars :rate="30" /></div>
              </b-col>
              <b-col lg="3" class="d-flex align-items-center skill-name">
                <div>SignalR</div>
                <div><Stars :rate="30" /></div>
              </b-col>
            </b-row>
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import Stars from "../components/Stars.vue";
export default {
  components: {
    Stars,
  },
};
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
  background-color: rgb(0 97 217);
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
  color: rgb(15 56 149);
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
  color: rgb(15 56 149);
}
.right-underline {
  width: 100%;
  height: 2px;
  margin-top: 5px;
  background-color: rgb(0 97 217);
}
.my-story {
  font-size: 16px;
  line-height: 26px;
  text-align: justify;
}
.soft-skill {
  height: 35px;
  border: 1px solid #ababff;
  border-left: 5px solid rgb(0 97 217);
  display: flex;
  align-items: center;
  border-radius: 5px;
  justify-content: flex-start;
  font-weight: 700;
  padding-left: 5px;
  cursor: pointer;
}
.soft-skill:hover {
  background: #ededff;
}
.skill-name {
  height: 35px;
  padding-left: 5px;
  border: 1px solid #ababff;
  border-left: 5px solid rgb(0 97 217);
  border-radius: 5px;
  font-size: 16px;
  font-weight: 700;
  cursor: pointer;
  justify-content: space-between;
  align-items: center;
}
.skill-name:hover {
  background: #ededff;
}
@media only screen and (max-width: 576px) {
  .main-style {
    padding: 5px;
  }
  .right-side {
    margin-top: 20px;
  }
  .soft-skill {
    margin-bottom: 20px;
  }
}
</style>
