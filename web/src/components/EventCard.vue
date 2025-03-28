<template>
    <v-card
      class="mx-auto"
      color="#36393f"
      max-width="650"
      min-height="350"
      theme="dark"
      variant="flat"
    >
      <v-sheet color="#202225">
        <v-card-item>
          <template v-slot:prepend>
            <v-card-title>
              <v-icon
                icon="mdi-email-arrow-right"
                start
              ></v-icon>
  
              Contact Me!
            </v-card-title>
          </template>
  
          <v-divider class="mx-2" vertical></v-divider>
  
          <a href="mailto:sunalng333@gmail.com">
            <v-btn
              class="text-none text-subtitle-1"
              color="#5865f2"
              size="small"
              variant="flat"
            >
              Send Email
            </v-btn>
          </a>
  
          <template v-slot:append>
          </template>
        </v-card-item>
      </v-sheet>
  
      <v-card
        class="ma-4"
        color="#2f3136"
        rounded="lg"
        variant="flat"
      >
        <v-card-item>
          <v-card-title class="text-body-2 d-flex align-center">
            <v-icon
              color="#949cf7"
              icon="mdi-at"
              start
            ></v-icon>
  
            <span class="text-medium-emphasis font-weight-bold">Tianhao Dong 董天灏</span>
  
            <v-spacer></v-spacer>
  
         <!--   <v-avatar
              image=" "
              size="x-small"
            ></v-avatar>
  -->
       <!--     <v-chip
              class="ms-2 text-medium-emphasis"
              color="grey-darken-4"
              prepend-icon="mdi-account-multiple"
              size="small"
              text="81"
              variant="flat"
            ></v-chip>-->
          </v-card-title>
  
          <div class="py-2">
            <div class="text-h6">Actively looking for a job</div>
  
            <div class="font-weight-light text-medium-emphasis">
                As an Information Systems graduate, I am eager to embark on my professional journey and embrace the opportunities and challenges that lie ahead. With a solid foundation in data analysis, system design, and project management, I am confident in my ability to contribute effectively to dynamic teams. My academic journey has equipped me with both technical expertise and critical thinking skills, which I believe are essential in today's fast-paced digital landscape where organizations increasingly rely on innovative solutions to drive growth. I am particularly excited about the prospect of working in roles such as Information Security Analyst or Data Scientist, fields that not only offer competitive salaries but also align with my passion for leveraging technology to solve complex problems. While I acknowledge the competitive nature of the job market, I am committed to continuously enhancing my skills—be it through advanced certifications or hands-on projects—to stay at the forefront of industry trends. Ultimately, I am looking forward to making a meaningful impact in my future workplace by turning ideas into actionable solutions and growing alongside a talented team.
            </div>
          </div>
        </v-card-item>
  
        <v-divider></v-divider>
  
        <div class="pa-4 d-flex align-center">
          <v-icon
            color="disabled"
            icon="mdi-wizard-hat"
            start
          ></v-icon>
  
          <v-icon
            color="disabled"
            icon="mdi-sword-cross"
          ></v-icon>
  
          <span class="text-caption text-medium-emphasis ms-1 font-weight-light">
            sunalng333@gmail.com
          </span>
  
          <v-spacer></v-spacer>
  
         <!-- <v-btn
            icon="mdi-dots-horizontal"
            variant="text"
          ></v-btn>
          -->
        <a href="https://github.com/SunLang333/">
          <v-btn
            class="me-2 text-none"
            color="#4f545c"
            prepend-icon="mdi-github"
            variant="flat"
          >
            Github
          </v-btn>
        </a>
        <a href="https://www.linkedin.com/in/dong-tianhao-6502b9217">
          <v-btn
            class="me-2 text-none"
            color="#4f545c"
            prepend-icon="mdi-linkedin"
            variant="flat"
          >
            Linkedin
          </v-btn>
        </a>
        </div>
      </v-card>
    </v-card>
  </template>