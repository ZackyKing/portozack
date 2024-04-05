<template>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css" integrity="sha512-SnH5WK+bZxgPHs44uWIX+LLJAJ9/2PkPKZ5QiAj6Ta86w+fsb2TkcmfRyVX3pBnMFcV7oQPJkl9QevSCWr3W6A==" crossorigin="anonymous" referrerpolicy="no-referrer" />
  <div id="header">
        <div class="container">
            <nav>
                <img src="./assets/Logo2.png" class="logo">
                <ul id="sidemenu">
                  <li><a href="#header" @click="scrollToSection('header')">Home</a></li>
                  <li><a href="#about" @click="scrollToSection('about')">About</a></li>
                  <li><a href="#services" @click="scrollToSection('services')">Service</a></li>
                  <li><a href="#portfolio" @click="scrollToSection('portfolio')">Project</a></li>
                  <li><a href="#contact" @click="scrollToSection('contact')">Contact</a></li>
                </ul>
            </nav>
            <div class="header-text">
                <p>UI/UX Designer & Programer</p>
                <h1>Hi, I'm <span>Zacky Argya Tarigan</span><br>Nice to meet you</h1>
            </div>
        </div>
    </div>
    <!-------------------------about----------------------------->
    <div id="about">
        <div class="container">
            <div class="row">
                <div class="about-col-1">
                    <img src="./assets/profile.png">
                </div>
                <div class="about-col-2">
                    <h1 class="sub-title">About me</h1>
                    <p>Hi, let me introduce myself, my name is ZackyArgyaTarigan. 
                      I am a student from Riau Islamic University, majoring in Computer 
                      Engineering. My journey is still long, and I aspire to become 
                      proficient in programming and design. My knowledge is not much yet, 
                      but as long as we keep learning, everything can be learned as long 
                      as there is determination from within oneself.
                    </p>

                        <div class="tab-titles">
                          <p class="tab-links" :class="{ 'active-link': activeTab === 'skills' }" @click="changeTab('skills')">Skills</p>
                          <p class="tab-links" :class="{ 'active-link': activeTab === 'experience' }" @click="changeTab('experience')">Experience</p>
                          <p class="tab-links" :class="{ 'active-link': activeTab === 'education' }" @click="changeTab('education')">Education</p>
                          <p class="tab-links" :class="{ 'active-link': activeTab === 'biodata' }" @click="changeTab('biodata')">Biodata</p>
                        </div>
                        <div class="tab-contents" :class="{ 'active-tab': activeTab === 'skills' }" id="skills">
                            <ul>
                                <li><span>UI/UX</span><br>Design Web/App Interfaces</li>
                                <li><span>Web Development</span><br>Web app Development</li>
                                <li><span>Game Development</span><br>Building&Desinging Desktop Games</li>
                            </ul>
                        </div>
                        <div class="tab-contents" :class="{ 'active-tab': activeTab === 'experience' }" id="experience">
                            <ul>
                                <li><span>HACKATON</span><br>Participate in Google HackFeast development</li>
                                <br>
                                <li><span>COMING SOON</span></li>
                            </ul>
                        </div>
                        <div class="tab-contents" :class="{ 'active-tab': activeTab === 'education' }" id="education">
                            <ul>
                                <li><span>SMA</span><br>SMA Negri 1 Rambah</li>
                                <li><span>Kuliah</span><br>Universitas Islam Riau</li>
                            </ul>
                        </div>
                        <div class="tab-contents" :class="{ 'active-tab': activeTab === 'biodata' }" id="biodata">
                            <ul>
                                <li><span>Nama</span><br>Zacky Argya Tarigan</li>
                                <li><span>Jenis Kelamin</span><br>Laki-laki</li>
                                <li><span>Tempat Lahir</span><br>Medan</li>
                                <li><span>Tanggal Lahir</span><br>26 Januari 2004</li>
                                <li><span>Pekerjaan</span><br>Mahasiswa</li>
                                <li><span>Kewarganegaraan</span><br>Indonesia</li>
                            </ul>
                        </div>
                </div>
            </div>
        </div>
    </div>
    <!-----------------------Servivces----------------------------------->
    <div id="services">
        <div class="container">
            <h1 class="sub-title">My Services</h1>
            <div class="services-list">
                <div>
                    <i class="fa-solid fa-code"></i>
                    <h2>Web Design</h2>
                    <p>I can design the website you desire, with a 
                      price that matches the skills I possess.</p>
                        <a href="#">Learn more</a>
                </div>
                <div>
                    <i class="fa-solid fa-crop"></i>
                    <h2>UI/UX Design</h2>
                    <p>I can design the UI/UX you desire. Although my skills 
                      may not yet match those of a professional, I can still 
                      make it beautiful.</p>
                        <a href="#">Learn more</a>
                </div>
                <div>
                    <i class="fa-solid fa-gamepad"></i>
                    <h2>Game Design</h2>
                    <p>I can design games, devise storylines, and create the games themselves with the 
                      skills I possess. I will continue to learn to compete with the professionals 
                      out there.</p>
                        <a href="#">Learn more</a>
                </div>
            </div>
        </div>
    </div>
    <!-------------------------Portofolio--------------------------------->
    <div id="portfolio">
        <div class="container">
            <h1 class="sub-title">My Work</h1>
            <div class="work-list">
                <div class="work">
                    <img src="./assets/mendignrp1.png">
                    <div class="layer">
                        <h3>Mobile App Mending Rakit PC #1</h3>
                        <p>"This is a prototype of an application I've created titled 
                          'Mending Rakit PC', which aims to help people 
                          assemble their own PCs without confusion and without 
                          falling victim to dishonest individuals."</p>
                            <a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                    </div>
                </div>
                <div class="work">
                    <img src="./assets/mendignrp2.png">
                    <div class="layer">
                        <h3>Mobile App Mending Rakit PC #2</h3>
                        <p>"This is a prototype of an application I've created titled 
                          'Mending Rakit PC', which aims to help people 
                          assemble their own PCs without confusion and without 
                          falling victim to dishonest individuals."</p>
                            <a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                    </div>
                </div>
                <div class="work">
                    <img src="./assets/mendignrp3.png">
                    <div class="layer">
                        <h3>Mobile App Mending Rakit PC #3</h3>
                        <p>"This is a prototype of an application I've created titled 
                          'Mending Rakit PC', which aims to help people 
                          assemble their own PCs without confusion and without 
                          falling victim to dishonest individuals."</p>
                            <a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                    </div>
                </div>
                <div class="work">
                    <img src="./assets/AgroSmart1.png">
                    <div class="layer">
                        <h3>AgroSmart Gardening App #1</h3>
                        <p>AgroSmart is an application developed by the ECHO team, aimed at facilitating 
                          farmers or plant enthusiasts out there. It includes features such as mobile 
                          monitoring, scheduled watering, and more.</p>
                            <a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                    </div>
                </div>
                <div class="work">
                    <img src="./assets/AgroSmart2.png">
                    <div class="layer">
                        <h3>AgroSmart Gardening App #2</h3>
                        <p>AgroSmart is an application developed by the ECHO team, aimed at facilitating 
                          farmers or plant enthusiasts out there. It includes features such as mobile 
                          monitoring, scheduled watering, and more.</p>
                            <a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                    </div>
                </div>
                <div class="work">
                    <img src="./assets/AgroSmart3.png">
                    <div class="layer">
                        <h3>AgroSmart Gardening App #3</h3>
                        <p>AgroSmart is an application developed by the ECHO team, aimed at facilitating 
                          farmers or plant enthusiasts out there. It includes features such as mobile 
                          monitoring, scheduled watering, and more.</p>
                            <a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                    </div>
                </div>
                <div class="work">
                    <img src="./assets/LegendOfGrym.png">
                    <div class="layer">
                        <h3>Game Development</h3>
                        <p>This is a game I've designed using the Scratch application, called 
                          'Legend Of Grym,' which tells the story of a young swordsman named 
                          Grym, on a quest to rescue a princess kidnapped by the demon king XOR. 
                          The game is still in the prototype stage, and I hope that in the future, 
                          I can create a game that is even better and more popular among many people.</p>
                            <a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                    </div>
                </div>
            </div>
            <a href="#" class="btn">See more</a>
        </div>
    </div>
    <!---------------------Contact------------------------------>
    <div id="contact">
        <div class="container">
            <div class="row">
                <div class="contact-left">
                    <h1 class="sub-title">Contact Me</h1>
                    <p><i class="fa-solid fa-paper-plane"></i> zackyargya@gmail.com</p>
                    <p><i class="fa-solid fa-square-phone"></i> 082155180690</p>
                    <div class="social-icons">
                        <a href="https://www.facebook.com/people/Zacky-Argya-Tarigan/pfbid038A7UmMVUEuzyZf4Y7fKHCuBnJH7B5e6rUkWKn9rrv18i6t5Z6FJvWkmrWUWBLZyRl/"><i class="fa-brands fa-facebook"></i></a>
                        <a href="https://www.instagram.com/zackyargyatarigan/"><i class="fa-brands fa-instagram"></i></a>
                        <a href="https://www.linkedin.com/in/zacky-argya-tarigan-52a296184/"><i class="fa-brands fa-linkedin"></i></a>
                        <a href="https://github.com/ZackyKing"><i class="fa-brands fa-github"></i></a>
                    </div>
                    <a href="./assets/background.png" download class="btn btn2">Download CV</a>
                </div>
                <div class="contact-right">
                    <form>
                        <input type="text" name="Name" placeholder="Your Name" required>
                        <input type="email" name="Email" placeholder="Your Email" required>
                        <textarea name="Massage" rows="6" placeholder="Your Message"></textarea>
                        <button type="submit" class="btn btn2">Submit</button>
                    </form>
                </div>
            </div>
        </div>
        <div class="copyright">
            <p>Copyright © ZackyArgyaTarigan.</p>
        </div>
    </div>
</template>

<script>
export default {
  data() {
    return {
      activeTab: 'skills' // Set initial active tab
    };
  },
  methods: {
    changeTab(tabName) {
      this.activeTab = tabName;
    },
    scrollToSection(sectionId) {
      const element = document.getElementById(sectionId);
      if (element) {
        element.scrollIntoView({ behavior: "smooth" });
      }
    }
  }
};
</script>

<style>
*{
  margin: 0;
  padding: 0;
  font-family: 'Poppins', sans-serif;
  box-sizing: border-box;
}
html{
  scroll-behavior: smooth;
}
body{
  background-color: #080808;
  color: #fff;
}
#header{
  width: 100%;
  height: 100vh;
  background-image: url(./assets/background.png);
  background-size: cover;
  background-position: center;
}
.container{
  padding: 10px 10%;
}
nav{
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
}

.logo{
  display: flex;
  width: 30vh;
}

nav ul li{
  display: inline-block;
  list-style: none;
  margin: 10px 20px;
}

nav ul li a{
  color: #fff;
  text-decoration: none;
  font-size: 18px;
  position: relative;
}
nav ul li a::after{
  content: '';
  width: 0;
  height: 3px;
  background: #ff004f;
  position: absolute;
  left: 0;
  bottom: -6px;
  transition: 0.5s;
}
nav ul li a:hover::after{
  width: 100%;
}
.header-text{
  margin-top: 20%;
  font-size: 30px;
}
.header-text h1{
  font-size: 45px;
  margin-top: 20px;
}
.header-text span{
  color: aqua;
}
/*----------about---------*/
#about{
  padding: 80px 0;
  color: #ababab;
}
.row{
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}
.about-col-1{
  flex-basis: 35%;
}
.about-col-1 img{
  width: 100%;
  border-radius: 15px;
}
.about-col-2{
  flex-basis: 60%;
}
.sub-title{
  font-size: 60px;
  font-weight: 600;
  color: #fff;
}
.tab-titles{
  display: flex;
  margin: 20px 0 40px;
}
.tab-links{
  margin-right: 50px;
  font-size: 18px;
  font-weight: 500;
  cursor: pointer;
  position: relative;
}
.tab-links::after{
  content: '';
  width: 0;
  height: 3px;
  background: #ff004f;
  position: absolute;
  left: 0;
  bottom: -8px;
  transition: 0.5s;
}
.tab-links.active-link::after{
  width: 50%;
}
.tab-contents ul li{
  list-style: none;
  margin: 10px 0;
}
.tab-contents ul li span{
  color: #b54769;
  font-size: 14px;
}
.tab-contents{
  display: none;
}
.tab-contents.active-tab{
  display: block;
}

/*-------------Service---------*/
#services{
  padding: 30px 0;
}
.services-list{
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  grid-gap: 40px;
  margin: 50px;
}
.services-list div{
  background: #262626;
  padding: 40px;
  font-size: 13px;
  font-weight: 300;
  border-radius: 10px;
  transition: background 0.5s, transform 0.5s;
}
.services-list div i{
  font-size: 50px;
  margin-bottom: 30px;
}
.services-list div h2{
  font-size: 30px;
  font-weight: 500;
  margin-bottom: 15px;
}
.services-list div a{
  text-decoration: none;
  color: #fff;
  font-size: 12px;
  margin-top: 20px;
  display: inline-block;
}
.services-list div:hover{
  background: #ff004f;
  transform: translateY(-10px);
}
/*----------------Portfolio---------------*/
#portfolio{
  padding: 50px 0;
}
.work-list{
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  grid-gap: 40px;
  margin-top: 50px;
}
.work{
  border-radius: 10px;
  position: relative;
  overflow: hidden;
}
.work img{
  width: 100%;
  border-radius: 10px;
  display: block;
  transition: transform 0.5s;
}
.layer{
  width: 100%;
  height: 0;
  background: linear-gradient(rgba(0,0,0,0.6), #ff004f);
  border-radius: 10px;
  position: absolute;
  left: 0;
  bottom: 0;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  padding: 0 40px;
  text-align: center;
  font-size: 14px;
  transition: height  0.5s;
}
.layer h3{
  font-weight: 500;
  margin-bottom: 20px;
}
.layer a{
  margin-top: 20px;
  color: #ff004f;
  text-decoration: none;
  font-size: 18px;
  line-height: 60px;
  background: #fff;
  width: 60px;
  height: 60px;
  border-radius: 50%;
  text-align: center;
}
.work:hover img{
  transform: scale(1.1);
}
.work:hover .layer{
  height: 100%;
}
.btn{
  display: block;
  margin: 50px auto;
  width: fit-content;
  border: 1px solid #ff004f;
  padding: 14px 50px;
  border-radius: 6px;
  text-decoration: none;
  color: #fff;
  transition: background 0.5s;
}
.btn:hover{
  background: #ff004f;
}

/*--------------contact--------------*/
.contact-left{
  flex-basis: 35%;
}
.contact-right{
  flex-basis: 60%;
}
.contact-left p{
  margin-top: 30px;
}
.contact-left p i{
  color: #ff004f;
  margin-right: 15px;
  font-size: 25px;
}
.social-icons{
  margin-top: 30px;
}
.social-icons a{
  text-decoration: none;
  font-size: 30px;
  margin-right: 15px;
  color: #ababab;
  display: inline-block;
  transition: transform 0.5s;
}
.social-icons a:hover{
  color: #ff004f;
  transform: translateY(-5px);
}
.btn.btn2{
  display: inline-block;
  background: #ff004f;
}
.contact-right form{
  width: 100%;
}
form input, form textarea{
  width: 100%;
  border: 0;
  outline: none;
  background: #262626;
  padding: 15px;
  margin: 15px 0;
  color: #fff;
  font-size: 18px;
  border-radius: 6px;
}
form btn2{
  padding: 14px 60px;
  font-size: 18px;
  margin-top: 20px;
  cursor: pointer;
}
.copyright{
  width: 100%;
  text-align: center;
  padding: 25px 0;
  background: #262626;
  font-weight: 300;
  margin-top: 20px;
}
/*-----------------css for small screens---------------*/
</style>

