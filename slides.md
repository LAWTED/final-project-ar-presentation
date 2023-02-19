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
  <video src="/cloud_computer.mp4" class="rounded-xl w-1/2 object-scale-down" controls></video>
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
layout: section
---
# Early-term Progress Report 🐦

---
layout: two-cols
---

# Overview

> successfully deployed a cloud page that is able to track the hiro marker and change the color of the cloud based on the sky color.


* ✅ Deploy on the website
* ✅ Model cloud track the hiro marker
* ✅ Sky color detection
* ✅ Cloud color change based on the sky color


::right::

<div class="w-full h-full flex justify-center items-center">
  <video src="/early-progress-report-overview.mp4" class="rounded-xl w-1/2 object-scale-down" controls></video>
</div>

---
layout: section
---

# Challenges


---
layout: two-cols
---

## tracking.js track preset color

```mermaid
graph TD
    A(View) -->|Get main color| B(Main color)
    B -->|track preset color| C(Know state when color find)
```

::right::

## Sky color detection

```mermaid
graph TD
    E(View) -->|Sky part filter| A(Sky View) -->|Get main color intime| B(Sky main color)
    B -->|set main color to cloud| C(Cloud color)
```


---
layout: two-cols
---

# Tracking.js in detecting weather

> use tracking.js to track some color but it's not accurate enough, and hard to tell the difference

tracking.js can track

* similar color 🟡
* color position ❌

But what we need

* tracking specific color 🔵


:: right ::

<div class="w-full h-full flex justify-center items-center">
  <video src="/tracking-yellow-color.mp4" class="rounded-xl w-1/2 object-scale-down" controls></video>
</div>

<!-- The limitations of tracking.js in detecting weather with the camera -->
---

# Identifying various shades of blue

<div class="grid grid-cols-2 gap-2">
  <div class="flex align-center gap-2">
    <div class="bg-[#5da8d0] w-min rounded-lg text-white p-1 my-auto"> #5da8d0 </div>
    <img src="/frames/frame0.jpg" class="rounded-xl w-64 object-scale-down" controls />
  </div>

  <div class="flex align-center gap-2">
    <div class="bg-[#4393be] w-min rounded-lg text-white p-1 my-auto"> #4393be </div>
    <img src="/frames/frame125.jpg" class="rounded-xl w-64 object-scale-down" controls />
  </div>

  <div class="flex align-center gap-2">
    <div class="bg-[#4184b4] w-min rounded-lg text-white p-1 my-auto"> #4184b4 </div>
    <img src="/frames/frame250.jpg" class="rounded-xl w-64 object-scale-down" controls />
  </div>

  <div class="flex align-center gap-2">
    <div class="bg-[#286ba4] w-min rounded-lg text-white p-1 my-auto"> #286ba4 </div>
    <img src="/frames/frame375.jpg" class="rounded-xl w-64 object-scale-down" controls />
  </div>

  <div class="flex align-center gap-2">
    <div class="bg-[#04548d] w-min rounded-lg text-white p-1 my-auto"> #04548d </div>
    <img src="/frames/frame500.jpg" class="rounded-xl w-64 object-scale-down" controls />
  </div>

  <div class="flex align-center gap-2">
    <div class="bg-[#1b233c] w-min rounded-lg text-white p-1 my-auto"> #1b233c </div>
    <img src="/frames/frame625.jpg" class="rounded-xl w-64 object-scale-down" controls />
  </div>
</div>

---

# Identifying various shades of blue

tracking method use rgb and the difference between red and blue or green and blue, or the distance between source color and the tracked color, and both two method can't track specific color and tell the shade of blue which we need


```js{7-9|10}
tracking.ColorTracker.registerColor('yellow', function(r, g, b) {
  var threshold = 50,
    dx = r - 255,
    dy = g - 255,☁️
    dz = b - 0;

  if ((r - b) >= threshold && (g - b) >= threshold) {
    return true;
  }
  return dx * dx + dy * dy + dz * dz < 10000;
});
```

<!-- The first method is using a threshold value of 50 to check if the difference between the red and blue color values is greater than or equal to the threshold, and if the difference between the green and blue color values is greater than or equal to the threshold. If both of these conditions are true, then the function will return true to indicate that the color is yellow.

The second method is using a "distance" formula to calculate the distance between the given color (r, g, b) and the color white (255, 255, 0). If this distance is less than 10000, then the function will again return true to indicate that the color is yellow.
 -->


<!-- The difficulty of accurately identifying various shades of blue and black using the RGB color space -->


---
layout: two-cols
---

# Impact of buildings

<!-- The impact of buildings on the screen on the tracking of main colors -->

the buildings on the screen will affect the tracking of main colors, and the color is not smoothly change


**The lack of existing solutions for sky detection using browser-based JavaScript implementation**

[![cftang0827/sky-detector - GitHub](https://gh-card.dev/repos/cftang0827/sky-detector.svg?fullname=)](https://github.com/cftang0827/sky-detector)

[![MaybeShewill-CV/sky-detector - GitHub](https://gh-card.dev/repos/MaybeShewill-CV/sky-detector.svg?fullname=)](https://github.com/MaybeShewill-CV/sky-detector)


::right::

<div class="w-full h-full flex justify-center items-center">
  <video src="/impact-building.mp4" class="rounded-xl w-1/2 object-scale-down" controls></video>
</div>

---
layout: section
---

# Solutions


---
layout: two-cols
---

<div class="opacity-30">

## tracking.js track preset color


```mermaid
graph TD
    A(View) -->|Get main color| B(Main color)
    B -->|track preset color| C(Know state when color find)
```

</div>

::right::

## Sky color detection

```mermaid
graph TD
    E(View) -->|Sky part filter| A(Sky View) -->|Get main color intime| B(Sky main color)
    B -->|set main color to cloud| C(Cloud color)
```

---

# Sky Part filter

* Use of opencv.js for more advanced image processing instead of simply tracking specific colors,

* Use of image segmentation and sky detection techniques, including the use of a Laplacian filter to extract parts of the image with lower variance than a threshold

* World First Sky Detection Using JavaScript

```js
const getSkyRegionGradient = (src, mask, h, w) => {
  let imgGray = new cv.Mat();
  cv.cvtColor(src, imgGray, cv.COLOR_RGBA2GRAY, 0);

  cv.blur(imgGray, imgGray, kSize);
  cv.medianBlur(imgGray, imgGray, 5);
  let lap = new cv.Mat();
  cv.Laplacian(imgGray, lap, cv.CV_8U, 1, 1, 0, cv.BORDER_DEFAULT);
  let gradient_mask = new cv.Mat();
  cv.threshold(lap, gradient_mask, 6, 255, cv.THRESH_BINARY_INV);
  let M = cv.Mat.ones(9, 3, cv.CV_8U);
  cv.erode(gradient_mask, mask, M);
  imgGray.delete();
  lap.delete();
  calSkyLine(mask, h, w);
};
```

---

# Sky Part filter

the sky part filter will get the sky part of the image

<br/>

<video src="/skyline.mp4" class="rounded-xl object-scale-down" autoplay loop></video>


---

# Sky Part filter

the main color of the sky part change smoothly

<video src="/sky-filter-main-color.mp4" class="rounded-xl object-scale-down" autoplay loop></video>

---

# Get main color realtime

use a class written by `whoiam2007s` to track the main color of the sky part, but change the input image type from canvas image to uint8array


[![whoiam2007s/ImgMainColor - GitHub](https://gh-card.dev/repos/whoiam2007s/ImgMainColor.svg?fullname=)](https://github.com/whoiam2007s/ImgMainColor)

```js{1-8|9}
new ImgMainColor(
  {
    imageData: skyView,
  },
  function (color) {
    const { hex } = color
    currentColor.style.backgroundColor = hex;
    currentColor.innerHTML = hex;
    model.attributes['light'].value = `type: ambient; color: ${hex}`;
  }
);
```

---
layout: section
---

# 后续可能遇到的问题和思考

---
layout: two-cols
---

# Cloud ☁

* 云彩的多角度打光进行拟真, 太阳光和天空环境光
* 通过AI可以通过天空识别当前时间和太阳角度
* 如何将标识和主体进行融合
* ...

::right::

# Animal 🦏

* 动物的声音识别可能需要用到AI技术, 待学习🧑‍💻
* ...


---
layout: section
---


# Mid-term Progress Report 🏃‍♂️


---
layout: two-cols
---
# Overview

> successfully implement the sky color detection, main color detection and surrounding volume meter.

* ✅ Implement the main page
* ✅ Cloud page color detect
* ✅ Fox model and animation
* ✅ volume meter
* ✅ Fox animate when volume meter change

::right::

<div class="w-full h-full flex justify-center items-center">
  <iframe src="https://cloud.lawted.tech" class="h-full w-2/3 rounded-xl"></iframe>
</div>

---
layout: section
---

# Finished work

---
layout: two-cols
---

# Main Page

> main page use the motion sensor to control the object view and click the button to redirect to the page

* 🏃‍♂️ View by Motion Sensor
* 🖐️ Scale by Finger Touch
* 🔘 Click the Button to Redirect to the Page

::right::

<div class="w-full h-full flex justify-center items-center">
  <video src="/main-page.mp4" class="rounded-xl w-1/2 object-scale-down" controls autoplay loop></video>
</div>




---
layout: two-cols
---

# Cloud Page

> Cloud model currently replaced by a box entity, because of the volume effect in `gltf` format has not solved yet

* ☁️ Deploy the Cloud Page
* 🎨 Track the Main Color of the Screen and Change the Color of the Cloud
* 🖌️ Main Color Detect will Filter Black and White Color
* ⚙️ Orbit Control the Object and Scale by Finger Touch

::right::

<div class="w-full h-full flex justify-center items-center">
  <video src="/cloud-page.mp4" class="rounded-xl w-1/2 object-scale-down" controls autoplay loop></video>
</div>

---
layout: two-cols
---

# Fox Page

> Fox model currently has three animation, survey, walk and run.


<div class="flex justify-between w-100 mt-10">
  <h3>
    low
  </h3>
  <h2>
    Volume
  </h2>
  <h3 >
    high
  </h3>
</div>

<div class="flex border-light-500 border-2 rounded-lg justify-between my-1 w-min ">
  <div class="bg-gray-400 rounded-l-md w-30 text-center"> survey </div>
  <div class="bg-green-400 w-30 text-center"> walk </div>
  <div class="bg-red-400 rounded-r-md w-40 text-center"> run </div>
</div>

* 🦊 Deploy the Fox Page
* 🔊 Volume Meter will Detect the Surrounding
* 🎥 Animation will Change when Volume Meter Changes
* ⚙️ Orbit Control the Object and Scale by Finger Touch

::right::

<div class="w-full h-full flex justify-center items-center">
  <video src="/fox-page.mp4" class="rounded-xl w-1/2 object-scale-down" controls autoplay loop></video>
</div>

---

# Work to do

* use shader to implement the cloud effect (volume ray cast effect)
  * learn shader and glsl language
  * implement the cloud effect with shaderMaterial

* use AI to detect the voice and change the animation of the fox
  * learn AI and tensorflow.js
  * deploy the AI model to the web

---
layout: two-cols
---

# Problems

```mermaid
flowchart LR
    A(Blender) -->|volume effect| B(Volume Model)
    B -->|No | C(GLTF format Cloud)
    A --> |Pure mesh| D(Mesh Model)
    D --> |Yes| C
```

::right::

<div class="w-full h-full flex justify-center items-center">
  <video src="/impact-building.mp4" class="rounded-xl w-1/2 object-scale-down" autoplay loop controls></video>
</div>



<!-- Blender is a popular 3D modeling software that allows users to create various models, including
cloud models. However, when it comes to deploying a cloud model on a website, it is important to choose the correct file format.
One such file format is glTF, which is specifically designed for efficient transmission and loading of 3D scenes and models on the web. Unfortunately, when exporting a cloud model from Blender to glTF format, there may be issues with the volume effect not being correctly represented. Therefore, while it is possible to shape a cloud model in Blender, it may not be currently possible to export it as a glTF file and deploy it on a website without the volume effect issues being addressed first.
 -->

---
layout: two-cols
---

# Solutions


use `shaderMaterial` construct a realtime cloud model which use `shader` language `glsl`, but it  can not reflected light now


```js
const vertexShader = /* glsl */ `...`
const fragmentShader = /* glsl */ `...`

const geometry = new THREE.BoxGeometry(1, 1, 1);
const material = new THREE.RawShaderMaterial({
  glslVersion: THREE.GLSL3,
  uniforms: {
    ...
  },
  vertexShader,
  fragmentShader,
  side: THREE.BackSide,
  transparent: true,
});
const mesh = new THREE.Mesh(geometry, material);

```

::right::

<div class="w-full h-full flex justify-center items-center">
  <img src="/shader-cloud.jpeg"  class="rounded-xl w-1/2 object-scale-down">
</div>



---
layout: quote
---

# "Thanks for your listening!"
