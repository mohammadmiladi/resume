<template>
  <div class="main-style">
    <b-container>
      <div class="projects mb-3">
        <div>About Me</div>
        <img src="@/assets/images/arr.png" width="80" alt="arrow" />
      </div>
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
              <b-row
                class="w-100 mb-3 g-2"
                style="justify-content: space-between"
              >
                <b-col lg="3" class="soft-skill">Project management</b-col>
                <b-col lg="3" class="soft-skill">Strong decision maker</b-col>
                <b-col lg="3" class="soft-skill">Complex problem solver</b-col>
              </b-row>
              <b-row class="w-100 g-2" style="justify-content: space-between">
                <b-col lg="3" class="soft-skill">Teamwork</b-col>
                <b-col lg="3" class="soft-skill">Fast Learner</b-col>
                <b-col lg="3" class="soft-skill">Motivated</b-col>
              </b-row>
            </div>
            <div class="right-title">
              <div>My Programming Skills</div>
              <div class="right-underline"></div>
            </div>
            <b-row
              class="w-100 mb-3 g-2"
              style="justify-content: space-between"
            >
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
            <b-row
              class="w-100 mb-3 g-2"
              style="justify-content: space-between"
            >
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
            <b-row
              class="w-100 mb-3 g-2"
              style="justify-content: space-between"
            >
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
            <b-row class="w-100 g-2" style="justify-content: space-between">
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
    <b-container>
      <div class="projects">My Projects</div>
      <div class="arrows">
        <div
          class="stacks"
          :style="projectName == 'react' && 'background: #8785ff'"
          @click="changeStack('react')"
        >
          <div>React</div>
          <img
            class="stack-logo"
            src="@/assets/images/react.png"
            alt="react-logo"
          />
        </div>
        <img
          class="arrow-width"
          src="@/assets/images/left.png"
          alt="left-arrow"
        />
        <img
          class="arrow-width"
          src="@/assets/images/right.png"
          alt="right-arrow"
        />
        <div
          class="stacks"
          :style="projectName == 'vue' && 'background: #8785ff'"
          @click="changeStack('vue')"
        >
          <div>Vue</div>
          <img
            class="stack-logo"
            src="@/assets/images/vue.png"
            alt="vue-logo"
          />
        </div>
      </div>
      <b-row v-if="projectName == 'vue'" class="g-3" style="min-height: 400px">
        <b-col lg="4">
          <div class="project">
            <div class="project-title">KookBaz Admin Panel</div>
          </div>
        </b-col>
        <b-col lg="4">
          <div class="project">
            <div class="project-title">IvaBit Admin Panel</div>
          </div>
        </b-col>
        <b-col lg="4">
          <div class="project">
            <div class="project-title">ParsToys Admin Panel</div>
          </div>
        </b-col>
        <b-col lg="4">
          <div class="project">
            <div class="project-title">BitBarg</div>
          </div>
        </b-col>
        <b-col lg="4">
          <div class="project">
            <div class="project-title">Landak</div>
          </div>
        </b-col>
        <b-col lg="4">
          <div class="project">
            <div class="project-title">Trustio</div>
          </div>
        </b-col>
        <b-col lg="4">
          <div class="project">
            <div class="project-title">DadBanan Dana</div>
          </div>
        </b-col>
        <b-col lg="4">
          <div class="project">
            <div class="project-title">Biz School</div>
          </div>
        </b-col>
      </b-row>
      <b-row
        v-if="projectName == 'react'"
        class="g-3"
        style="min-height: 400px"
      >
        <b-col lg="4">
          <div class="project">
            <div class="project-title">Kookbaz Shop</div>
            <div></div>
          </div>
        </b-col>
        <b-col lg="4">
          <div class="project">
            <div class="project-title">Tehran Swimming Questionnaire</div>
          </div>
        </b-col>
        <b-col lg="4">
          <div class="project">
            <div class="project-title">IvaBit</div>
          </div>
        </b-col>
        <b-col lg="4">
          <div class="project">
            <div class="project-title">
              FootBall Resualt Monitoring (practice)
            </div>
          </div>
        </b-col>
        <b-col lg="4">
          <div class="project">
            <div class="project-title">Todo list (Practice)</div>
          </div>
        </b-col>
      </b-row>
    </b-container>
    <b-container>
      <div class="projects mb-3">
        <div>Contact Me</div>
        <img src="@/assets/images/arr.png" width="80" alt="arrow" />
      </div>
      <div class="contacts">
        <b-row style="width: 100%">
          <form ref="form" @submit.prevent="sendEmail">
            <b-col lg="12">
              <div>
                <div>Name:</div>
                <div>
                  <input
                    class="input-style"
                    name="user_name"
                    type="text"
                    placeholder="Name"
                  />
                </div>
              </div>
            </b-col>
            <b-col lg="12">
              <div>
                <div>Email:</div>
                <div>
                  <input
                    class="input-style"
                    name="user_email"
                    type="email"
                    placeholder="Email"
                  />
                </div>
              </div>
            </b-col>
            <b-col lg="12">
              <div>
                <div>Subject:</div>
                <div>
                  <input
                    name="user_subject"
                    class="input-style"
                    type="text"
                    placeholder="Subject"
                  />
                </div>
              </div>
            </b-col>
            <b-col lg="12">
              <div>
                <div>Message:</div>
                <div>
                  <textarea
                    class="input-style"
                    name="message"
                    placeholder="Message"
                    id=""
                    cols="30"
                    rows="10"
                  ></textarea>
                </div>
              </div>
            </b-col>
            <div>
              <button type="submit" class="submit-style">Submit</button>
            </div>
          </form>
        </b-row>
      </div>
    </b-container>
  </div>
</template>

<script>
import Stars from "../components/Stars.vue";
import emailjs from "@emailjs/browser";

export default {
  components: {
    Stars,
  },
  data() {
    return {
      projectName: "vue",
    };
  },
  methods: {
    changeStack(payload) {
      this.projectName = payload;
    },
    sendEmail() {
      emailjs
        .sendForm(
          "service_ur4zlos",
          "template_mz49st8",
          this.$refs.form,
          "user_KLqzX4eym7Xj5H5GOEQnL"
        )
        .then(
          (result) => {
            console.log("SUCCESS!", result.text);
          },
          (error) => {
            console.log("FAILED...", error.text);
          }
        );
    },
  },
};
</script>

<style scoped>
@font-face {
  font-family: "SFPro";
  src: local("SFPro"), url(../assets/fonts/SFPro.ttf) format("truetype");
}
* {
  scroll-behavior: smooth;
  font-family: "SFPro";
}
.arrows {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 40px;
}
.arrow-width {
  width: 100px;
}
.stack-logo {
  width: 50px;
}
.project-title {
  font-weight: 700;
  margin-bottom: 20px;
}
.stacks {
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
  margin: 20px;
  padding: 10px 30px;
  background: white;
  border-radius: 5px;
  font-weight: 700;
}
.stacks:hover {
  background: whitesmoke;
}
.projects {
  width: 100%;
  margin-top: 40px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: max-content;
  font-weight: 700;
  font-size: 40px;
}
.input-style {
  width: 100%;
  border: 1px solid rgb(201, 201, 201);
  border-radius: 4px;
  padding: 5px;
}
.input-style:focus {
  outline: none;
}
.submit-style {
  background-color: rgb(63, 63, 180);
  color: white;
  border: 1px solid rgb(53, 53, 194);
  border-radius: 5px;
  padding: 5px 12px;
}
.contacts {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  height: max-content;
  font-weight: 700;
  box-shadow: 0px 40px 64px -12px rgba(0, 0, 0, 0.08),
    0px 0px 14px -4px rgba(0, 0, 0, 0.05), 0px 32px 48px -8px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
  padding: 25px;
  background-color: white;
}
.project {
  box-shadow: 0px 40px 64px -12px rgba(0, 0, 0, 0.08),
    0px 0px 14px -4px rgba(0, 0, 0, 0.05), 0px 32px 48px -8px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
  padding: 25px;
  background-color: white;
  display: flex;
  justify-content: center;
  align-items: center;
}
.main-style {
  padding: 0 50px;
  min-height: 100vh;
  height: 100%;
  overflow-x: hidden;
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
  min-height: 767px;
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
  margin: 30px 0;
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
  .arrow-width {
    width: 70px;
  }
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
  .arrow-width {
    width: 50px;
  }
  .stacks {
    padding: 10px;
  }
  .stack-logo {
    width: 30px;
  }
}
</style>
