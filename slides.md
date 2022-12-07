---
theme: apple-basic
lineNumbers: true
drawings:
  persist: false
layout: intro
title: Final Project Presentation
---

# Final Project Presentation

Applying AR technology for art exhibition on Mobile devices

<div class="absolute bottom-10">
  <span class="font-700">
    Wu Mingze
  </span>
</div>

<!--
Hello, everyone, I am Wu Mingze, and i am gonna talk about my final project which is applying AR technology for artexhibiton on Mobile devices
-->

---
layout: intro-image-right
image: /ar.jpg
---

# Augmented Reality

an interactive experience that combines the real world and computer-generated content.

<!--
First, AR as Augmented Reality is different from VR, VR is something u put a vr headsets on, such as pico4 from bytedance or quest pro from meta. And when u put the headsets on, u diverse into a virtual world like "Ready Player One", a film by Spielberg on 2018. That's VR, and AR is to combine the real world and computer-generated content, which means u can see overlay of generated content by screen and the real world by camera
-->

---
layout: section
---

# The Outcomes

<!--
Second I am gonna talk about the outcoms
-->

---
layout: two-cols
---

# Cloud

<br/>
<br/>
displaying the AR subject (cloud)

which colors will change according to the light shifting in the surrounding environment
<br/>

<img src="/cloud.png" class="rounded w-100 h-60 object-cover"/>

::right::

# Animal

<br/>
<br/>
displaying the AR subject (animal)

which forms will change according to the sound trigger from the surrounding environment
<br/>

<img src="/animal.png" class="rounded w-100 h-60 object-cover"/>

<!--
the project is applying ar technology to a art exhibiton, and i am gonna show two pilot demo, one is a cloud and the other is an animal, moreover, the cloud needs to change according to the light shifting, which is the hardest part in this project. And the animal will interact with the ambient sound, if u talk loud maybe the animal will scared or angry. something like this. So a full animation for the animal is needed.
-->

---
layout: section
---

# Stacks

<!--
third part is about the stacks and the technology section
-->

---

# AR SDK Technology Selection

* ARCore  <PajamasGoogle/> with kotlin <LogosKotlinIcon/> for Android
* ARKit   <CibApple/> with swift <LogosSwift/> for iOS
* AR Foundation <LogosUnity/> with C# for Unity, Android and iOS
* Ar.js <LogosJavascript/> with three.js <LogosThreejs/> for web, Android and iOS

<!--
first thing first, how to find the write ar sdk techonology which is Suitable for the exhibiton. well i think if no need to install the program, it is best not to install it. And It's best that everyone can use it on their mobile phones whether it's Apple or Android because as cindy said this will literally apply to a exhibition and its a demo for bussiness not a demo for study. so if it is a app, i need to learn arcore with kotlin and arkit with swift. and when user use it they need to download app i think that makes the project too heavy. i prefer to make the project light to use. so i choose the last one. one more thing i also consider to use miniprogram from wechat but its on beta version and there are a lot of limits, but if it goes well, the program will also be ported to the wechat
-->

---

# Modeling Technology Selection

* blender <LogosBlender/>

<br/>
<br/>

<img src="https://i.all3dp.com/wp-content/uploads/2022/01/31151522/3d-print-with-blender-aftab-ali-via-all3dp-220114.jpg" class="rounded w-120 object-cover"/>

<!--
second one is modeling, i choose blender definitely, because i used it before and i think its the best modeling software for small model
-->

---

# Tracking Technology Selection

* tracking.js

<br/>
<br/>

<img src="/tracking.png" class="rounded w-120 object-cover"/>

<!--
third part is tracking, the cloud should track the light, and i do a lot of reseach, the light should change its color instead of change its intensity. first, not every phone has a ambient light sensor, second AR requires stable light intensity for positioning, hence here i will use tracking.js to track the colors from the camera. u can see it can circle the colors of yellow and purple
-->

---
layout: two-cols
---
# Audio Technology Selection

* Audioworklet

::right::

<iframe src="https://goblin-laboratory.github.io/volume-meter/" class="rounded w-full h-full object-cover" allow='microphone'></iframe>

<!--
fourth is audio technology, i will use audioworklet for tracing the volume, it is common that many online meeting has this feature, u speak and u can see the voulme from your micphone that is base on the audioworklet
-->

---

# Final stack section

<br/>
<br/>

AR.js + blender <LogosBlender/> + three.js <LogosThreejs/> + tracking.js + webRTC <LogosWebrtc/>

<br/>

Ar.js for AR content

blender for 3D modeling

three.js for 3D rendering

tracking.js for color tracking

webRTC for video streaming

<!--
now let me make a summary, i am going to build a webpage which can run on any browser, and use these stacks to build it.
-->

---

# Timeline


```mermaid
gantt
    title Final Project AR Timeline
    dateFormat  YYYY-MM-DD
    section Background
    Study AR technologies in web domain :a1, 2022-11-01, 45d
    Study AR technologies in Mobile Natives :a2, 2022-11-16  , 30d
    Step up environment :a3, 2022-11-16 , 45d
    Release the first version of the demo :a4, 2022-12-01, 30d
    Simple page :milestone, 2022-12-15, 0d


    section Cloud
    Modeling a cloud :b1, 2022-12-01, 90d
    Deploy the cloud into web page     :b1, 2022-12-01  , 90d
    Track the video from camera :b3, 2022-12-16 , 75d
    Bind the state :b4, 2023-01-01, 60d
    Cloud page :milestone, 2023-01-16, 0d

    section Animal
    Modeling a animal :c1, 2023-01-16, 75d
    Deploy the cloud into web page     :c1, 2023-02-01  , 59d
    Track the light from camera :c3, 2023-02-01 , 59d
    Voice detection :c4, 2023-01-16, 75d
    Animal page :milestone, 2023-3-01, 0d

    section Deploy
    Deploy the website :d1, 2022-12-01, 150d
    CDN optimize :d2, 2023-03-15, 15d
    Generate user guide :d3, 2023-02-16, 75d
    Make a demo video :d4, 2023-04-01, 30d
    Full page :milestone, 2023-03-20, 0d

    section Feedback
    feedback round 1 :e1, 2022-12-16, 15d
    feedback round 2 :e2, 2023-01-16, 15d
    feedback round 3 :e2, 2023-02-16, 15d
    feedback round 4 :e2, 2023-03-16, 15d

```
---
layout: section
---

# 12/07 Demo 🧑‍💻

<!--
OK, i am gonna tell u my current progress and follow-up plans, because my project is a engineer instead of a research hence let's just forward to the result.
-->

---
layout: two-cols
---

# Cloud 🌩️

* link: [cloud.lawted.tech](https://cloud.lawted.tech)
* track HIRO marker


<img src="/hiro.jpg" class="w-80 h-80 object-cover ">

::right::

<div class="w-full h-full flex justify-center items-center">
  <video src="/cloud_computer.MP4" class="rounded-xl w-1/2 object-scale-down" controls></video>
</div>

<!--
take a look at the video on the left, this is a screenshoot on my phone and u can see the cloud is stick on the hiro marker. and when we walk to another direction the cloud won't rotate but show another aspect
-->

---

# Blend the cloud model

* [cloud.blend](https://sketchfab.com/3d-models/cloud-3a76eb255e3c4c0199bbfedb2b54342f)

<br/>

<img src="/cloud_blender.jpg" class="rounded w-120 object-cover"/>

<!--
i download the cloud model and it looks great in the modeling software
-->

---
layout: two-cols
---

# AR.js to position the cloud

* hiro marker is used to position the cloud

<br/>
<br/>

```html {8|4-9|all}
<!-- main code -->
...
    <a-scene embedded arjs>
    <a-marker preset="hiro">
        <a-entity
        position="-0.5 1.5 0"
        scale="0.3 0.3 0.3"
        gltf-model="/cloud.gltf"
        ></a-entity>
    </a-marker>
    <a-entity camera></a-entity>
    </a-scene>
...
```

::right::

<div class="w-full h-full flex justify-center items-center">
  <img src="/corner.png" class="rounded w-9/10 object-cover"/>
</div>

<!--
second part is track by ar.js, here is part of the code we export the cloud to gltf format and use a-marker to position it
-->

---
layout: two-cols
---

# deploy the page

* use tencent cloud server to deploy the page
* use nginx to add ssl certificate
* enable to use on phone and computer in browser

```nginx
server {
    listen 443 ssl;
    server_name cloud.lawted.tech;
    ssl_certificate /etc/nginx/ssl/cloud.lawted.tech/fullchain.cer;
    ssl_certificate_key /etc/nginx/ssl/cloud.lawted.tech/cloud.lawted.tech.key;
    ssl_session_timeout 5m;
    ssl_protocols TLSv1 TLSv1.1 TLSv1.2;
    ssl_ciphers ALL:!ADH:!EXPORT56:RC4+RSA:+HIGH:+MEDIUM:+LOW:+SSLv2:+EXP;
    ssl_prefer_server_ciphers on;
    location / {
        root /var/www/cloud;
        index index.html index.htm;
    }
}
```

::right::


<div class="w-full h-full flex justify-center items-center">
  <img src="/cloud_phone.jpg" class="rounded w-1/2 object-cover"/>
</div>

<!--
final part is deploy the page, now its on my website and because if the website need to control the camera it should be cetificate by ssl and deploy as a https website
-->

---
layout: bullets
---

# Next step improvement

* add more cloud models and make them move

* use track.js to track the light and make the cloud change its color

<!--
add more status of cloud, such as clouds in morning and afternoon and eve

second thing is use track.js to track the color change in the video.
-->

---
layout: quote
---

# "Thanks for your listening!"
