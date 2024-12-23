# Nmap
Adwance nmap scaning for information gathring





How to install NMAP in Termux?
The process of Termux Nmap installation is as easy as installing any other package in termux. we will update our termux before installing it so we don't face any bugs.

Step 1:

Nmap is a really important tool and we don't want any bugs while running it so we will first upgrade the packages using the below command.
```
apt update && apt upgrade -y
```
How to Install and Use Nmap In Termux - 2024
This command will Install updates in all the previously installed packages in termux.



Step 2:

Nmap is just a basic Package in termux and you can install it like any other package so To install Nmap in Temux you just have to use the pkg command. Nmap is a small package so it won't take a lot of data to download it. You can just paste the below command and it will be installed in no time.
```
pkg install nmap -y
```
How to Install and Use Nmap In Termux - 2024
Now if you see the $ sign on your Termux that means its Completely installed.



NOTE: This post is only for educational purposes. I and this site do not support any criminal activity. If you are doing any sort of misuse of this information This site is not responsible for that. THIS SITE ONLY SUPPORT ETHICAL HACKING. 




Common Nmap Commands in Termux :
You can do many things with the help of the Nmap tool but in Termux Nmap tutorial, I am gonna give few important commands that will give a brief idea of how you can use the Nmap tool in termux.
How to scan a Website with Nmap Termux :
To scan a Website you must have permissions Else it can cause you Trouble, Nmap allows you to Scan there Test website so, in this post, we will use that website, you just have to type Nmap and then the site name you can paste the below command in the termux to scan the Nmap test website.
```
nmap Scanme.nmap.org
```
How to Install and Use Nmap In Termux - 2024
 

Output :

You can see that we got an IP-Adress of the website in the second line as well as we can see the latency is 0.24 Seconds.and we can also see all the open port of the website.

Nmap in Termux command output



Scan your Local Network with Nmap Termux :
If You just wanna scan your Local network (Your Intire subnet )and know How many devices are connected with your Wifi then you can use this command. This command will give you a list of all Devices in the network as well as you all the open ports of those devices.
```
nmap 192.168.1.1/24
```
How to Install and Use Nmap In Termux - 2025
 

 Output :

Now you can see in the below picture, I have 2 devices in my network. and you can also see all the open ports. The 192.168.1.202 Host is up and the latency is 0.0025s. If you have multiple devices on your network then it will show you a list of all the Devices.

Nmap in Termux command output

# Advanced Nmap Usage:
While basic scans can provide useful information, Nmap shines when you explore its advanced features. These advanced techniques can help you uncover deeper insights about the network, operating systems, and services running on hosts. Let’s explore a few key advanced Nmap commands.
Aggressive scan using Nmap Termux :
Aggressive scans provide detailed information about the target, including OS detection, version detection, script scanning, and traceroute. This is useful when you need to gather comprehensive details.
```
nmap -A 192.168.1.1/24
```
How to Install and Use Nmap In Termux - 2025
 

Output :

With the aggressive scan, you can see more details like the iBall Baton Login and the URL of the login page. This example is from my local network, so you might not find anything too exciting. However, when scanning a website, this command can uncover a lot more useful information.

Nmap in Termux command output


Operating System Detection (-O):
Nmap can attempt to detect the operating system of a host based on network responses. This is handy for network administrators or ethical hackers looking to understand the target’s OS.

```
nmap -O scanme.nmap.org
```
Output :

Nmap will analyze network packets and return the most likely operating system and its version. While not always 100% accurate, it provides valuable insights. 




Scan a Single port in Nmap Termux :
If you just wanna scan a Single Port of a Particular Ip address then you can do that using the below command. Here I am scanning the entire network for the port 80 but you can put a single IP and it will work Perfectly. The advantage of scanning a single port is that it will save you some extra time especially when you are in a hurry.
````
nmap -p 80 192.168.1.1/24
````
How to Install and Use Nmap In Termux - 2025
 

Output :

Here you can see that Nmap is checking for port 80 only but on my entire network.

Nmap in Termux command output


Scan Multiple Port in Nmap Termux :
Do you know most of the time when you scan a Network and you find a device with open port 80 as well as 443 then it means that its a WebServer? So In the below command, I am gonna scan these two ports on my network, of course, I don't have a webserver running in my home so it won't show 443 port but if you scan it in a network where they have a webserver then it will show with this command.
```
nmap -p 80,443 192.168.1.1/24
````
How to Install and Use Nmap In Termux - 2025
 

Output :

In the below picture you can clearly see that it is only checking for 2 port and as the output, we can see in my routers Ip address port 80 is open but port 443 is not. And in my second device, Both ports are closed.

Nmap in Termux command output





Ping A Website or an IP-Address with NMAP in Termux :
If you Quickly wanna Check if a Host is still up or not then you can do a Ping. It will tell you the amount of time it took the Nmap to make a connection with the website or the Device.
````
nmap -sP 192.168.1.202
````
How to Install and Use Nmap In Termux - 2025
You can also Type Nmap -sP www.google.com and it will ping the google server and tell you latency. 

Output :

You can see that the latency is 0.02 seconds and the Host is still up.

Nmap in Termux command output



Perform a Quick Scan with NMAP in Termux:
If you just wanna do a quick scan of the network and you only wanna know basic information then you can use -F Argument. It is much faster than the normal scan.
````
nmap -F 192.168.1.1/24
````
How to Install and Use Nmap In Termux - 2025
 

 Output :

Here you can see I got the output much faster and The result is still good.

Nmap in Termux command output



Check Nmap Version in Termux :
If you wanna check the Nmap Version then you can type the below command.
```
nmap -V
```
How to Install and Use Nmap In Termux - 2025
 

Output :

Now you can see the Nmap Version in the below picture.

Nmap in Termux command output



Conclusion :
Nmap is a Fine information gathering tool and it can be useful for people who are at least


<img align="center" height="auto"
src="https://cardivo.vercel.app/api?name=𝕄ℝ-VISHWAJIT&description=Hi,%20i%27m%20a%20Student%20and%20programer%20Nice%20to%20meet%20you%20👋&image=https://blogger.googleusercontent.com/img/a/AVvXsEjKJE35baqUfHK_30VA3kgzvoBn2P0ejulETazoiZdyYkvCuUl5Z8uw8C0zBD03C0Pyg6Hqxt0Z5md4de3mBIKoBZtJ4ns4hKZ71X9rsbzOpJlzqZqatEUknHGfKW6Us5FDpl5q48WExeN4FR_csq-pyncjw1fQ0bl2-2xP4lLnY-L8saho9FMKo8lIBJAQ?v=4&backgroundColor=%23ecf0f1&github=Vishwajitji&pattern=leaf&colorPattern=%23eaeaea"/>

<p align="center"> 
 
 

 
 [![Vishwajitji](https://readme-typing-svg.demolab.com?font=Anton&size=30&pause=1000&width=480&lines=Hello+everyone;My+name+is+VISHWAJIT;I+am+from+India+(Uttar+Pradesh)+;Nice+to+meet+you)](https://git.io/typing-svg)

p align="center"> 
  Visitor Count<br>
  <img src="https://profile-counter.glitch.me/Vishwajitji/count.svg" />
</p>

 <p align="center">
  
[![Typing SVG](https://readme-typing-svg.demolab.com?font=Anton&weight=480&size=30&pause=1000&color=FF00BE&width=435&lines=Hello%2C+I+am+Smart+Boy;Don't+Follow+Me;You+are+Hacked)](https://git.io/typing-svg)

<p align="center">


<h1 align="center">Hi 👋, My name is Vishwajit</h1>
<h3 align="center">I'm a student</h3>



## My Programming Stats

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Exo+2&size=24&duration=4000&pause=1000&color=03F700&center=true&vCenter=true&width=320&lines=%F0%9F%98%87++Welcome++%F0%9F%98%87;I+Love+My+India;You+Are+Hacked;Nice+To+Meet+You)](https://git.io/typing-svg)


<p align="left"> <a href="https://www.11ty.dev/" target="_blank" rel="noreferrer">
  



<p><img align="center" src="https://github-readme-stats.vercel.app/api/top-langs?username=Vishwajitji&show_icons=true&locale=en&layout=compact" alt="Vishwajitji" /></p>

<p>&nbsp;<img align="left" src="https://github-readme-stats.vercel.app/api?username=Vishwajitji&show_icons=true&locale=en" alt="Vishwajitji" /></p>






| <img align="center" width="100%" src="https://github-readme-stats.vercel.app/api?username=Tohidkhan6332&count_private=true&include_all_commits=true&show_icons=true&theme=blue-green&border_color=001F1E&text_color=09d672&icon_color=00C2C2&title_color=00F1E9&custom_title=Stats" alt="My GitHub Stats" /> <img align="center" width="100%" src="https://github-readme-stats.vercel.app/api/wakatime?username=gamemann&theme=blue-green&border_color=001F1E&text_color=09d672&icon_color=00C2C2&title_color=00F1E9" alt="My GitHub Time Stats" /> 










<p align="center">
  <a href="https://github.com/DenverCoder1/readme-typing-svg">
    <img src="https://readme-typing-svg.herokuapp.com?font=Time+New+Roman&color=cyan&size=25&center=true&vCenter=true&width=600&height=100&lines=Assalamu+O+Alaikum+Warahmatullah..&hearts;++;Self-taught+Back-End+Developer,;Engineering+Student,;My+Hobby+Is+Coding,;Active+Learner/Researcher,;Love+to+learn+new+stuffs..<3">
  </a>
</p>


---

## 📊 Languages and Tools
<img align="right" width="40%" src="https://media.giphy.com/media/YxdQy6Vxbvb44/giphy.gif" alt="Basecamp sky" />

<img alt="Development" width="250" src="https://media2.giphy.com/media/W9tBvzTXkQopi/giphy.gif?cid=6c09b952xu6syi1fyqfyc04wcfk0qvqe8fd7sop136zxfjyn&ep=v1_internal_gif_by_id&rid=giphy.gif&ct=g" /> </p>


# 📫 How to reach me:

[![Via WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/+919559099482?text=Hello+Hacker)

[![MY Telegram](https://img.shields.io/badge/telegram-1b77FF.svg?style=for-the-badge&logo=telegram)](https://t.me/Rv99482) 

---

## <div align="center">🌱 Social Networks:
  </div>

<p align="left">
<a href="https://x.com/RV4685291395252/status/1844200187465773503" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="https://x.com/RV4685291395252/status/1844200187465773503" height="30" width="40" /></a>
<a href="https://www.facebook.com/share/1Adjrcrwxb/" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/facebook.svg" alt="Vishwajit Kushwaha" height="30" width="40" /></a>
<a href="https://www.instagram.com/smartboy.coming?igsh=cTMzbnQ3dmk4eDJj" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="Vishwajitji" height="30" width="40" /></a>
</p>

 <div id="badges" align="center">
    <a href="https://www.github.com/Vishwajitji" target="_blank">
      <img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/github-dark.svg" width="40" height="40" alt="Github"/>
    </a>
    <a href="https://in.linkedin.com/in/ravi-kumar-bb8ba92a8" target="_blank">
      <img src="https://cdn-icons-png.flaticon.com/512/2504/2504799.png" width="40" height="40" alt="linkedin" />
    </a>
    <a href="https://www.youtube.com/@onlinecoursebestchanal" target="_blank">
      <img src="https://cdn-icons-png.flaticon.com/512/3670/3670147.png" width="40" height="40" alt="Youtube"/>
    </a>
  </div>

---

# ⚡ Vishwajit INFO


- 😊 I’m Vishwajit
- 👦🏻 Age is unknown
- 👀 I’m interested in Hacking,Programming,Javascript ,bot deployment,python,C...
- 🌱 Currently a student at unknown
- 💞️ I’m looking to collaborate on programming ,Linux ,Linux tools development ,WhatsApp bot development...
- 📫 Email me via rraj6741660@gmail.com to contact
- 🤩 Follow me on Instagram https://www.instagram.com/smartboy.coming?igsh=cTMzbnQ3dmk4eDJj
- 💬 Text me on telegram https://t.me/Rv99482
- ✉️ Text me on WhatsApp https://api.whatsapp.com/send/?phone=919559099482



