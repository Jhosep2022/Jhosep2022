[<p align="center">
  <img src="https://github.com/thompsonemerson/thompsonemerson/raw/master/cover-thompson.png" height="200"/>
</p>

<!--horizontal divider(gradiant)-->
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">

<!--h1 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h1 style="display: inline-block">Hi 👋, I'm Jose Condori</h1></summary>
  </ul>
</div>

<br/>

<p align="center">
	<a href="https://github.com/Bouaskaoun">
		<img src="https://readme-typing-svg.herokuapp.com?lines=Developer+Mobile;Full+Stack+Web+Developer;Freelancer;DS%20|%20AI%20|%20ML%20Enthusiastic;Always%20learning%20new%20things&center=true&width=380&height=45">
	</a>
</p>

<!--h2 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h2 style="display: inline-block">Confusion is part of Programming</h2></summary>
  </ul>
</div>

<!--Intro start-->
- 🔭 I’m currently working on **AWS, Angular, Flutter, Spring Boot JAVA, MongoDB, Postgres, Docker, Python, Nextjs**

- 🌱 I’m currently learning **to put together multiple Hyper Beast Stack for Scalable Applications.**

- ☁️ I've keen interest in cloud computing. So, I'm learning **AWS, Firebase, Cloud, IA**

- 📝 I regularly read articles on [Hashnode](https://fullstackopen.com/es/)

- 💬 Ask me about **Flutter, Angular, Vue.js, nodejs, mongoDB, Spring Boot JAVA**

- 📫 Feel free to reach me out **amadeo74080986@gmail.com**

<!--Intro end-->

<!--- stats & Trophy (start) -->
<p align="center">
<table align="center">
<tr border="none">
<td width="50%" align="center">
  <img  align="center" src="https://github-readme-stats.vercel.app/api?username=Bouaskaoun&theme=dark&show_icons=true&count_private=true" />
  <br><br>
  <img  title="🔥 Get streak stats for your profile at git.io/streak-stats" alt="Mark streak" src="https://github-readme-streak-stats.herokuapp.com/?user=Bouaskaoun&theme=dark&hide_border=false" /> 
</td>

<td width="50%" align="center">
  <img  align="center" src="https://github-readme-stats.anuraghazra1.vercel.app/api/top-langs/?username=Bouaskaoun&theme=dark&hide_border=false&no-bg=true&no-frame=true&langs_count=10"/>
</td>
</tr>
</table>
</p>        
<!--- stats (end) -->

<!--h1 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h2 style="display: inline-block">Technologies That I Know👨🏻‍💻</h2></summary>
  </ul>
</div>

<!--tech stack icons-->
<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=git,aws,bootstrap,c,cpp,css,discord,docker,dynamodb,express,figma,firebase,github,html,idea,java,js,kotlin,linux,materialui,mongodb,mysql,nextjs,nodejs,postman,py,react,redux,tailwind,ts,flutter,dart,tensorflow,redis,nginx,vuejs,vscode&perline=14" />
  </a>
</p>

<!--- snake (official placement) -->
## 🐍 My Contribution Snake

<p align="center">
  <img src="https://github.com/Bouaskaoun/Bouaskaoun/blob/output/github-contribution-grid-snake.svg" alt="snake animation" />
</p>

<!--profile visit count-->
<div align="center">
  [![](https://visitcount.itsvg.in/api?id=Bouaskaoun&icon=3&color=6)](https://visitcount.itsvg.in)
</div>

<!--horizontal divider(gradiant)-->
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">

<!-- Connect with me -->
<!--h2 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h2 style="display: inline-block">Connect With Me🤝</h2></summary>
  </ul>
</div>

<!--icons and links-->
<p align="center">
<a href="https://www.linkedin.com/in/jose-amadeo-condori-ramos-890bb3257/" target="blank"><img align="center" src="https://user-images.githubusercontent.com/88904952/234979284-68c11d7f-1acc-4f0c-ac78-044e1037d7b0.png" alt="linkedin" height="50" width="50" /></a>
<a href="https://twitter.com/amadeo_con62956" target="blank"><img align="center" src="https://user-images.githubusercontent.com/88904952/234980676-61bfb021-ecc8-48f7-88e6-34c1b06c4a58.png" alt="twitter" height="50" width="50" /></a> 
<a href="https://www.instagram.com/jose.ramos.2000/" target="blank"><img align="center" src="https://user-images.githubusercontent.com/88904952/234981169-2dd1e58f-4b7e-468c-8213-034ba62156c3.png" alt="instagram" height="50" width="50" /></a>
<a href="mailto:amadeo740809865@gmail.com" target="_blank">
  <img align="center" src="https://user-images.githubusercontent.com/88904952/234982196-562aea17-5532-4550-8c08-1c7cb994a541.png" alt="Enviar mensaje" height="50" width="50" />
</a>
</p>
](https://raw.githubusercontent.com/Bouaskaoun/Bouaskaoun/output/github-contribution-grid-snake.svg

me sale nof found por que no usaste el que mostre


name: generate animation

on:
  # run automatically every 24 hours
  schedule:
    - cron: "0 */24 * * *" 
  
  # allows to manually run the job at any time
  workflow_dispatch:
  
  # run on every push on the master branch
  push:
    branches:
    - master
    
  

jobs:
  generate:
    permissions: 
      contents: write
    runs-on: ubuntu-latest
    timeout-minutes: 5
    
    steps:
      # generates a snake game from a github user (<github_user_name>) contributions graph, output a svg animation at <svg_out_path>
      - name: generate github-contribution-grid-snake.svg
        uses: Platane/snk/svg-only@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
          
          
      # push the content of <build_dir> to a branch
      # the content will be available at https://raw.githubusercontent.com/<github_user>/<repository>/<target_branch>/<file> , or as github page
      - name: push github-contribution-grid-snake.svg to the output branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

este qie te dogie 

<p align="center">
  <img src="https://github.com/thompsonemerson/thompsonemerson/raw/master/cover-thompson.png" height="200"/>
</p>
<!--horizontal divider(gradiant)-->
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">


<!--h1 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h1 style="display: inline-block">Hi 👋, I'm Jose Condori</h1></summary>
  </ul>
</div>
<br/>
<p align="center">
	<a href="https://github.com/Bouaskaoun">
		<img src="https://readme-typing-svg.herokuapp.com?lines=Developer+Mobile;Full+Stack+Web+Developer;Freelancer;DS%20|%20AI%20|%20ML%20Enthusiastic;Always%20learning%20new%20things&center=true&width=380&height=45">
	</a>
</p>

<!--h2 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h2 style="display: inline-block">Confusion is part of Programming</h2></summary>
  </ul>
</div>


<!--Intro start-->
- 🔭 I’m currently working on **AWS, Angular, Flutter, Spring Boot JAVA, MongoDB, Postgres, Docker, Python, Nextjs**

- 🌱 I’m currently learning **to put together multiple Hyper Beast Stack for Scalable Applications.**

- ☁️ I've keen interest in cloud computing. So,I'm learning **AWS, Firebase, Cloud, IA**

- 📝 I regularly read articles on [Hashnode]([https://1010nishant.hashnode.dev/](https://fullstackopen.com/es/))

- 💬 Ask me about **Flutter, Angular, Vue.js, nodejs, mongoDB, Spring Boot JAVA**

- 📫 Feel free to reach me out **amadeo74080986@gmail.com**

<!--Intro end-->



<!--- stats & Trophy (start) -->
<p align="center">
  <!--- stats (start) -->
<table align="center">
<tr border="none">
<td width="50%" align="center">
  
  <img  align="center"  src="https://github-readme-stats.vercel.app/api?username=1010nishant&theme=dark&show_icons=true&count_private=true" />
  <br></br>
  <img  title="🔥 Get streak stats for your profile at git.io/streak-stats" alt="Mark streak" src="https://github-readme-streak-stats.herokuapp.com/?user=1010nishant&theme=dark&hide_border=false" /> 
</td>

<td width="50%" align="center">

  <img  align="center"  src="https://github-readme-stats.anuraghazra1.vercel.app/api/top-langs/?username=1010nishant&theme=dark&hide_border=false&no-bg=true&no-frame=true&langs_count=10"/>
  
  </td>
</tr>
</table>
<!--- stats (end) -->




</p>        
<!--- stats (end) -->


<!--h1 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h2 style="display: inline-block">Technologies That I Know👨🏻‍💻</h2></summary>
  </ul>
</div>
<!--tech stack icons-->
<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=git,aws,bootstrap,c,cpp,css,discord,docker,dynamodb,express,figma,firebase,github,html,idea,java,js,kotlin,linux,materialui,mongodb,mysql,nextjs,nodejs,postman,py,react,redux,tailwind,ts,flutter,dart,tensorflow,redis,nginx,vuejs,vscode&perline=14" />
  </a>

</p>


<!--- snake -->
<div align="center">
  <img src="https://raw.githubusercontent.com/Bouaskaoun/Bouaskaoun/output/github-contribution-grid-snake.svg" alt="snake animation"/>
</div>

<!--profile visit count-->
<div align="center">
  
[![](https://visitcount.itsvg.in/api?id=1010nishant&icon=3&color=6)](https://visitcount.itsvg.in)
  
</div>

<!--horizontal divider(gradiant)-->
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">

<!-- Connect with me -->
<!--h2 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h2 style="display: inline-block">Connect With Me🤝</h2></summary>
  </ul>
</div>


<!--icons and links-->
<p align="center">
<a href="https://www.linkedin.com/in/jose-amadeo-condori-ramos-890bb3257/" target="blank"><img align="center" src="https://user-images.githubusercontent.com/88904952/234979284-68c11d7f-1acc-4f0c-ac78-044e1037d7b0.png" alt="linkedin" height="50" width="50" /></a>
<a href="https://twitter.com/amadeo_con62956" target="blank"><img align="center" src="https://user-images.githubusercontent.com/88904952/234980676-61bfb021-ecc8-48f7-88e6-34c1b06c4a58.png" alt="twitter" height="50" width="50" /></a> 
<a href="https://www.instagram.com/jose.ramos.2000/" target="blank"><img align="center" src="https://user-images.githubusercontent.com/88904952/234981169-2dd1e58f-4b7e-468c-8213-034ba62156c3.png" alt="instagram" height="50" width="50" /></a>
<a href="mailto:amadeo740809865@gmail.com" target="_blank">
  <img align="center" src="https://user-images.githubusercontent.com/88904952/234982196-562aea17-5532-4550-8c08-1c7cb994a541.png" alt="Enviar mensaje" height="50" width="50" />
</a>
<!-- <a href="https://discord/jhosep#4394" target="blank"><img align="center" src="https://user-images.githubusercontent.com/88904952/234982627-019fd336-6248-453c-9b05-97c13fd1d207.png" alt="discord" height="50" width="50" /></a> -->
  
</p>
)
