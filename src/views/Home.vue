<template>
  <v-layout column class="mt-4 pt-2">
    <v-layout column justify-center align-center>
      <!-- <VueCompareImage
        class="hidden-md-and-down"
        hover
        :style="{ minWidth: '1300px' }"
        :sliderLineWidth="sliderLine"
        :handleSize="hSize"
        :leftImage="leftImage"
        :rightImage="rightImage"
        :sliderPositionPercentage="sliderPosition"
      />
      <VueCompareImage
        class="hidden-lg-and-up"
        hover
        :style="{ maxWidth: '400px' }"
        :sliderLineWidth="sliderLine"
        :handleSize="hSize"
        :leftImage="leftImage2"
        :rightImage="rightImage2"
        :sliderPositionPercentage="sliderPosition"
      /> -->
      <v-layout>
        <vue-responsive-image
          :image-url="imgbg"
          :image-ratio="9/16"
        ></vue-responsive-image>
        <!-- <img :src="imgbg" alt=""> -->
        <v-layout column justify-center align-center wrap class="mt-4 pt-2">
          <div v-responsive.lg.xl ><vue-typer class="headline" :repeat="0" text=" Ardyan Sabat Welly"></vue-typer></div>

          <div v-responsive.md    ><vue-typer class="headline" :repeat="0" text=" Ardyan Sabat Welly"></vue-typer></div>

          <div v-responsive.sm.xs ><vue-typer class="headline" :repeat="0" text="   Welly"></vue-typer></div>
            
          <div v-responsive.lg.xl >
            <vue-typer
              :text="text1"
              :repeat="Infinity"
              :shuffle="false"
              initial-action="erasing"
              :pre-type-delay="70"
              :type-delay="70"
              :pre-erase-delay="1980"
              :erase-delay="150"
              erase-style="select-back"
              :erase-on-complete="false"
              caret-animation="smooth"
            ></vue-typer>
          </div>
    
          <div v-responsive.md    >
            <vue-typer
              :text="text1"
              :repeat="Infinity"
              :shuffle="false"
              initial-action="erasing"
              :pre-type-delay="70"
              :type-delay="70"
              :pre-erase-delay="1980"
              :erase-delay="150"
              erase-style="select-back"
              :erase-on-complete="false"
              caret-animation="smooth"
            ></vue-typer>
          </div>
        </v-layout>
      </v-layout>
      <br>
      <div v-responsive.sm.xs >
        <vue-typer
              :text="text1"
              :repeat="Infinity"
              :shuffle="false"
              initial-action="erasing"
              :pre-type-delay="70"
              :type-delay="70"
              :pre-erase-delay="1980"
              :erase-delay="150"
              erase-style="select-back"
              :erase-on-complete="false"
              caret-animation="smooth"
            ></vue-typer>  
      </div>
      <v-flex xs12 sm6 md4 lg4 xl4>
        <v-card flat color="transparent" max-width="700">
          <v-card-title primary-title>
            <div>
              <h3 class="headline mb-0">
                <span>About</span>
                <span class="teal--text">Me</span>
              </h3>
              <div>
                <p>
                  Hi, my name Ardyan Sabat Welly.
                  I am a
                  <span
                    class="teal--text font-weight-bold"
                  >Accounting Supervisor at Piaggio Group</span>. Currently I work in Jakarta, Indonesia. 
                </p>
              </div>
            </div>
          </v-card-title>


          <v-card-actions class="hidden-sm-and-down">
            <v-btn
              v-for="icon in icons"
              :key="icon.icon"
              fab
              dark
              outline
              color="teal"
              :href="icon.href"
              target="_blank"
            >
              <v-icon dark>{{icon.icon}}</v-icon>
            </v-btn>
          </v-card-actions>

          <v-card-actions class="hidden-md-and-up justify-center">
            <v-btn
              v-for="icon in icons"
              :key="icon.icon"
              small
              fab
              dark
              outline
              color="teal"
              :href="icon.href"
              target="_blank"
            >
              <v-icon dark>{{icon.icon}}</v-icon>
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
    </v-layout>
    <v-layout row justify-center align-center wrap class="mt-4 pt-2">
      <v-flex xs12 sm12 md5 lg6 xl6 class="mt-4 pt-4">
        <h2 class="mb-4 pl-4 pt-2">Education</h2>
        <v-card-text class="py-0">
          <v-timeline align-top dense>
            <!-- <v-timeline-item color="teal" small>
              <v-layout pt-3>
                <v-flex xs4>
                  <div class="caption font-weight-bold teal--text">JAN 2018 -</div>
                  <div class="caption font-weight-bold teal--text">PRESENT</div>
                </v-flex>
                <v-flex class="pl-2">
                  <strong>Full Stack Web Development Course</strong>
                  <div class="caption mb-2">freeCodeCamp</div>
                </v-flex>
              </v-layout>
            </v-timeline-item> -->
  
            <v-timeline-item color="teal" small>
              <v-layout pt-3>
                <v-flex xs4>
                  <div class="caption font-weight-bold teal--text">2021 -</div>
                  <div class="caption font-weight-bold teal--text">2022</div>
                </v-flex>
                <v-flex class="pl-2">
                  <strong>Magister Akuntansi </strong>
                  <div>Atma Jaya Catholic University of Indonesia</div>
                  <!-- <div class="caption mb-2">Microsoft
                    <v-btn
                      href="https://drive.google.com/file/d/10qH597x_EBfJjwcyVZUiQBQA3Mt3r_VD/view?usp=share_link"
                      target="_blank"
                      color="teal"
                      dark
                      small
                    >
                      Certificate
                      <v-icon right dark>fas fa-file-download</v-icon>
                    </v-btn>
                  </div> -->
                </v-flex>
              </v-layout>
            </v-timeline-item>
  
            <v-timeline-item color="teal" small>
              <v-layout pt-3>
                <v-flex xs4>
                  <div class="caption font-weight-bold teal--text">2011 -</div>
                  <div class="caption font-weight-bold teal--text">2015</div>
                </v-flex>
                <v-flex class="pl-2">
                  <strong>Gelar Sarjana, Akuntansi dan Keuangan</strong>
                  <div class="caption">Universitas Advent Indonesia</div>
                  <div class="caption mb-2">Bachelor's degree - 3.61</div>
                </v-flex>
              </v-layout>
            </v-timeline-item>
          </v-timeline>
        </v-card-text>
      </v-flex>
      <v-flex xs12 sm12 md4 lg6 xl6 class="mt-4 pt-2">
        <h2 class="mb-4 pl-4">Experience</h2>
        <v-card-text class="py-0">
          <v-timeline align-top dense>
            <v-timeline-item color="teal" small>
              <v-layout pt-3>
                <v-flex xs4>
                  <div class="caption font-weight-bold teal--text">AUGUST 2019 -</div>
                  <div class="caption font-weight-bold teal--text">PRESENT</div>
                </v-flex>
                <v-flex class="pl-2">
                  <strong>Accounting Supervisor</strong>
                  <div class="caption mb-2">Piaggio Group - Jakarta</div>
                </v-flex>
              </v-layout>
            </v-timeline-item>

            <v-timeline-item color="teal" small>
              <v-layout pt-3>
                <v-flex xs4>
                  <div class="caption font-weight-bold teal--text">MAY 2018 -</div>
                  <div class="caption font-weight-bold teal--text">AUGUST 2019</div>
                </v-flex>
                <v-flex class="pl-2">
                  <strong>Capital Expenditure Specialist</strong>
                  <div class="caption mb-2">The Kraft Heinz Company - Jakarta</div>
                </v-flex>
              </v-layout>
            </v-timeline-item>

            <v-timeline-item color="teal" small>
              <v-layout pt-3>
                <v-flex xs4>
                  <div class="caption font-weight-bold teal--text">JUNE 2015 -</div>
                  <div class="caption font-weight-bold teal--text">MAY 2018</div>
                </v-flex>
                <v-flex class="pl-2">
                  <strong>Auditor</strong>
                  <div class="caption mb-2">Grant Thornton Indonesia - Jakarta</div>
                </v-flex>
              </v-layout>
            </v-timeline-item>

            <v-timeline-item color="teal" small>
              <v-layout pt-3>
                <v-flex xs4>
                  <div class="caption font-weight-bold teal--text">APRIL 2015 -</div>
                  <div class="caption font-weight-bold teal--text">MAY 2015</div>
                </v-flex>
                <v-flex class="pl-2">
                  <strong>Purchasing Staff</strong>
                  <div class="caption mb-2">PT. Agromas Group - Jakarta</div>
                </v-flex>
              </v-layout>
            </v-timeline-item>

            <v-timeline-item color="teal" small>
              <v-layout pt-3>
                <v-flex xs4>
                  <div class="caption font-weight-bold teal--text">MARCH 2015 -</div>
                  <div class="caption font-weight-bold teal--text">APRIL 2015</div>
                </v-flex>
                <v-flex class="pl-2">
                  <strong>Accounting Staff</strong>
                  <div class="caption mb-2">East Java Academy - Jawa Timiur</div>
                </v-flex>
              </v-layout>
            </v-timeline-item>
  
            <v-timeline-item color="teal" small>
              <v-layout pt-3>
                <v-flex xs4>
                  <div class="caption font-weight-bold teal--text">JUNE 2014 -</div>
                  <div class="caption font-weight-bold teal--text">JULY 2014</div>
                </v-flex>
                <v-flex class="pl-2">
                  <strong>Audit Staff</strong>
                  <div class="caption mb-2">KAP Rexon Nainggolan & Rekan - Jakara</div>                    
                </v-flex>
              </v-layout>
            </v-timeline-item>
  
            <v-timeline-item color="teal" small>
              <v-layout pt-3>
                <v-flex xs4>
                  <div class="caption font-weight-bold teal--text">MAY 2012 -</div>
                  <div class="caption font-weight-bold teal--text">JULY 2012</div>
                </v-flex>
                <v-flex class="pl-2">
                  <strong>Quality Monitoring Staff</strong>
                  <div class="caption mb-2">UT QUALITY INDONESIA, PT · Batam</div>
                </v-flex>
              </v-layout>
            </v-timeline-item>
          </v-timeline>
        </v-card-text>
      </v-flex>
    </v-layout>
    <h2 class="pl-4">
      <!-- <span>project</span>
      <span class="teal--text">My Own</span> -->
    </h2>
    <!-- <v-layout row justify-center align-center wrap class="mt-4 pt-2">
      <v-dialog
        v-model="project.dialog"
        lazy
        max-width="1000"
        v-for="project in projects"
        :key="project.title"
      >
        <template v-slot:activator="{ on }">
          <v-flex xs12 sm6 md4 lg4 xl4 v-on="on" >
            <v-card hover flat color="transparent"   class="m-4 p-2">
              <v-img
                :src="project.poster"
                :alt="project.title"
                width="90%"    
                lazy-src="https://cdn.dribbble.com/users/503653/screenshots/3143656/fluid-loader.gif"
              ></v-img>
              <v-card-title primary-title class="justify-center">{{project.title}}</v-card-title>
            </v-card>
          </v-flex>
        </template>
        <v-card v-if="project.dialog">
          <v-img :src="project.poster"></v-img>
          <v-card-text>
            <h3 class="headline mb-0">
              <span>Technology</span>
            </h3>
            <span v-for="(value, key) in project.tech"
             :key="key">
              <v-chip color="teal" text-color="white">{{value}}</v-chip>         
            </span>        
          </v-card-text>
          <v-card-actions>
            <v-btn large flat dark color="teal" :href="project.demo" target="_blank">
              <v-icon left>fas fa-desktop</v-icon>Demo
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-dialog>
    </v-layout> -->
    <h2 class="pl-4">
      <span>Latest </span>
      <span class="teal--text">Experience Information</span>
    </h2>
    <v-layout row justify-center align-center wrap class="mt-4 pt-2">
      <v-dialog
        v-model="project.dialog"
        lazy
        max-width="1000"
        v-for="project in projects_office"
        :key="project.title"
      >
        <template v-slot:activator="{ on }">
          <v-flex xs12 sm6 md4 lg4 xl4 v-on="on" >
            <v-card hover flat color="transparent"   class="m-4 p-2">
              <v-img
                :src="project.poster"
                :alt="project.title"
                width="90%"
               
                
                
                lazy-src="https://cdn.dribbble.com/users/503653/screenshots/3143656/fluid-loader.gif"
              ></v-img>
              <v-card-title primary-title class="justify-center">{{project.title}}</v-card-title>
            </v-card>
          </v-flex>
        </template>
        <v-card v-if="project.dialog">
          <v-img :src="project.poster"></v-img>
          <v-card-text>
            <h3 class="headline mb-0">
              <span>{{ project.job }}</span>
            </h3>

            <span v-for="(value, key) in project.tech"
             :key="key">
              <v-chip  color="teal" text-color="white">{{value}}</v-chip>
              <!-- <v-chip color="teal" text-color="white">{{project.tech.tech2}}</v-chip> -->
            </span>
            <div  class="mt-4 pt-2 pre-formatted " >{{ project.information }}</div>
            <!-- <v-chip color="teal" text-color="white">{{project.tech.tech3}}</v-chip>
            <v-chip color="teal" text-color="white">{{project.tech.tech4}}</v-chip> -->
          </v-card-text>
          <v-card-actions>
            <!-- <v-btn flat large dark color="teal" :href="project.git" target="_blank">
              <v-icon left>fab fa-github</v-icon>GitHub
            </v-btn> -->
            <!-- <v-btn large flat dark color="teal" :href="project.demo" target="_blank">
              <v-icon left>fas fa-desktop</v-icon>Demo
            </v-btn> -->
          </v-card-actions>
        </v-card>
      </v-dialog>
    </v-layout>
  </v-layout>
</template>

<script>
import { VueTyper } from "vue-typer";
import VueCompareImage from "vue-compare-image";
import VueResponsiveImage from 'vue-responsive-image';

export default {
  metaInfo: {
    title: "Home",
    titleTemplate: "%s ← welly's",
    meta: [
      { name: "viewport", content: "width=device-width, initial-scale=1" },
      { name: "description", content: "taro league Portfolio" },
      { charset: "utf-8" },
      { property: "og:title", content: "taro visual" },
      { property: "og:site_name", content: "taro visual" },
      { property: "og:type", content: "website" },
      { property: "og:url", content: "https://gomgomsihotang.site" },
      {
        property: "og:image",
        content: ""
      },
      { property: "og:description", content: "taro league Portfolio" }
    ]
  },
  components: {
    "vue-typer": VueTyper,
    VueCompareImage,
    VueResponsiveImage
  },
  data() {
    return {
      icons: [
        // { href: "https://github.com/gomxx2", icon: "fab fa-github" },
        // {
        //   href: "https://stackoverflow.com/users/story/9660700",
        //   icon: "fab fa-stack-overflow"
        // },
        // { href: "https://twitter.com/EldinMatricar", icon: "fab fa-twitter" },
        {
          href: "https://www.linkedin.com/in/ardyan-sabat-welly-20621ab1/",
          icon: "fab fa-linkedin-in"
        },
        // {
        //   href: "https://www.xing.com/profile/Eldin_Zaimovic?sc_o=mxb_p",
        //   icon: "fab fa-xing"
        // },
        // {
        //   href: "https://www.facebook.com/EldinVasVoli",
        //   icon: "fab fa-facebook-f"
        // },
        // {
        //   href: "https://www.youtube.com/channel/UC-IAD8yEJD-Mu6Y_56dVCtQ",
        //   icon: "fab fa-youtube"
        // },
        // {
        //   href: "https://www.youtube.com/channel/UC-IAD8yEJD-Mu6Y_56dVCtQ",
        //   icon: "fab fa-tiktok"
        // },
        // { href: "https://www.instagram.com/matricar", icon: "fab fa-instagram" }
      ],
      projects: [
         {
          dialog: false,
          title: "ngomong.online",
          git: "",
          demo: "http://ngomong.online/",
          tech: {
            tech1: "flask",
            tech2: "python",
            tech3: "Docker",
          },
          poster: require("../../public/img/example_ngomong.png")
        },
        {
          dialog: false,
          title: "Lagu Sion",
          // git: "https://github.com/EldinZaimovic/Eldin-Space-Vue",
          demo: "https://play.google.com/store/apps/details?id=com.lagu_sion",
          tech: {
            tech1: "dart",
            tech2: "flutter",
            tech3: "Play Store Publish from Flutter",
          },
          poster: require("../../public/img/lagusion_ex.png")
        },
        {
          dialog: false,
          title: "Slapur Church Hymnal",
          git: "https://cdn.neow.in/news/images/uploaded/2018/11/1543476286_cybersecurity.jpg",
          demo: "https://play.google.com/store/apps/details?id=com.slapur_church_hymnal",
          tech: {
            tech1: "dart",
            tech2: "flutter",
            tech3: "Play Store Publish from Flutter",
          },
          poster: require("../../public/img/sch_ex.png")
        },
       
      ],
      projects_office: [
         {
          dialog: false,
          job: "Accounting Supervisor",
          title: "Piaggio Indonesia",
          git: "",
          demo: "http://ngomong.online/",
          tech: {
            tech1: "excel",
          },
          information: "• Performing Finance, Accounting, and Tax duties using SAP system \n \
• Preparing month end journal entries timely and accurately in accordance with PSAK and TAX Regulation updated\n \
• Preparing daily reporting, consolidation and provide in depth financial analyst\n \
• Ensuring monthly financial statement report are precisely calculated and reported on time to the management (Balance Sheet, Income Statement, etc)\n \
• Ensuring that update documentation is always done every year\n \
• Oversees Accounting and Financing operations, which include financial accounting, tax setting in each invoice, accounts payable, and financial projections. Implements training for new hires and identifies training opportunities for current staff.",
          poster: require("../../public/img/piaggio_ex.png")
        },
        {
          dialog: false,
          job: "Capital Expenditure Specialist",
          title: "The Kraft Heinz Company",
          // git: "https://github.com/EldinZaimovic/Eldin-Space-Vue",
          demo: "https://play.google.com/store/apps/details?id=com.lagu_sion",
          tech: {
            tech1: "excel",
          },
          information: "Support Engineering Team :\n \
1. Provide detailed analysis/usage on Capex Budget and support manager to fully utilize all the Capex Budget Given for the Year.\n \
2. Prepare supporting data and support manager to calculate the Financial Return of a project before taking decision whether the project can go or postponed/cancelled.\n \
3. Oversee day to day 4site Capex Activity such as checking supporting document before upload into 4site, ensure the data is accurate and clear to understand, start the workflow of a project to listed approver. \n \
4. Along with Manager provide Financial support to Engineering Team when attending a monthly WHQ call for Capex Project above USD 250k and EVP Call (attended by Eduardo P and David Knopf) for Project above USD 1MM\n \
5. Provide supporting data to manager for all savings initiatives that is funded by Capex Budget make sure they will impact into company’s PL\n \
6. Provide support on analyzing maintenance expense if there’s a machine that can be replaced with a new one using Capex Budget.\n \
7. Lead Yearly Budgeting Process related to Capex Budget and make sure all the critical projects that is proposed by Engineering Team include in the budget.\n \
Financials & Reporting\n \
1. Supervise on closing and forecasting process related to Fixed Assets and Capex that is done by FXA/Capex Staff and Supervisor \n \
2. Deliver accurate and timely monthly financial reporting related to Fixed Assets and Capex which include Balance Sheet Account Reconciliation, P&L Accruals and Transactional Data Analysis.\n \
3. Prepare supporting data for Closing Deck, MPR and Supply Chain Deck related to Capex and Fixed Assets\n \
4. Fully aware on policy compliance related to Engineering area and ensure there’s no significant audit issue related to policy compliance (no Sox Deficiencies occurred) \n \
5. Provide support to Engineering Team if there’s any Audit Performed by External Parties (PwC) or Internal (Internal Audit) and also assist the auditor in Yearly Financial Audit Assessment",
          poster: require("../../public/img/kraftheinz_ex.png")        
        },
        {
          dialog: false,
          job: "Auditor",
          title: "Grant Thornton Indonesia",
          git: "https://cdn.neow.in/news/images/uploaded/2018/11/1543476286_cybersecurity.jpg",
          demo: "https://play.google.com/store/apps/details?id=com.slapur_church_hymnal",
          tech: {
            tech1: "excel",
          },
          information: "In general, trough cooperation of the rest of team member under the control of partner, manager and in charge personal (auditor) in certain project of client;\n \
1 The objective of the ordinary audit of financial statements by the independent auditor is the expression of an opinion on the fairness with which they present, in all material respects, financial position, results of operations, and its cash flows in conformity with generally accepted accounting principles.\n \
2 To plan and perform the audit to obtain reasonable assurance about whether the financial statements are free of material misstatement, whether caused by error or fraud. Because of the nature of audit evidence and the characteristics of fraud, the auditor is able to obtain reasonable, but not absolute.\n \
3 The auditor's responsibility is to express an opinion on the financial statements.\n \
4 The professional qualifications required of the independent auditor are those of a person with the education and experience to practice as such.\n \
5 In the observance of generally accepted auditing standards, the independent auditor must exercise his judgment in determining which auditing procedures are necessary in the circumstances to afford a reasonable basis for his opinion.\n \
Detection of Fraud (6-9)\n \
[Superseded January 1977 by Statement on Auditing Standards No. 16, as superseded by Statement on Auditing Standards No. 53, as superseded by section 316. Paragraphs renumbered by the issuance of Statement on Auditing Standards No. 82, February 1997.]\n \
10 The independent auditor also has a responsibility to his profession, the responsibility to comply with the standards accepted by his fellow practitioners. In recognition of the importance of such compliance, the American Institute of Certified Public Accountants has adopted, as part of its Code of Professional Conduct, rules which support the standards and provide a basis for their enforcement.\n \
Based on the SAS No. 1, section 110; SAS No. 78; SAS No. 82.",
          poster: require("../../public/img/grantthornton_ex.png")
        }
       
      ],
      text1: [" Atma Jaya Catholic University-Magister Akuansi", " Accounting Supervisor - Piaggio Group"],
      leftImage: require("../../public/img/1.png"),
      rightImage:require( "../../public/img/3.png"),
      imgbg:require("../../public/img/bgwelbgcool.png"),
      // leftImage2: require("../../public/img/3.png"),
      // rightImage2: require("../../public/img/2.png"),
      // leftImage: "https://i.xx.com/bU50uS9.jpg",
      // rightImage: "https://i.xx.com/z3ZoEEw.jpg",
      // leftImage2: "https://i.xx.com/z3ZoEEw.jpg",
      // rightImage2: "https://i.xx.com/Dcz2PGx.jpg",
      sliderLine: 0,
      hSize: 0,
      sliderPosition: 0.5
    };
  }
};
</script>
<style>
.pre-formatted {
  white-space: pre-wrap;
}

@keyframes rocking {
  0%,
  100% {
    transform: rotateZ(-10deg);
  }

  50% {
    transform: rotateZ(10deg);
  }
}

.vue-typer {
  font-family: Arial, "Helvetica Neue", Helvetica, sans-serif;
}
.vue-typer .custom.char.typed {
  color: #009688;
}
.vue-typer .custom.char.selected {
  color: #e91e63;
}

.vue-typer .custom.caret {
  animation: rocking 1s ease-in-out 0s infinite;
}
.vue-typer .custom.caret.typing {
  background-color: #009688;
}
.vue-typer .custom.caret.selecting {
  display: inline-block;
  background-color: #e91e63;
}
</style>

