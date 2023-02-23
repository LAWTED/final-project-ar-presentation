---
theme: apple-basic
lineNumbers: true
drawings:
  persist: false
layout: section
title: Final Project Presentation
transition: fade-out
download: true
css: unocss
---

# Applying AR technology for art exhibition on Mobile devices

##  Mid-term Progress Report 🏃‍♂️

<div class="absolute bottom-10">
  <span class="font-700">
    Wu Mingze
  </span>
</div>

<!--
Dear audience,

I am excited to share with you the mid-term progress report of my project, which focuses on applying AR technology for art exhibition on mobile devices.

My project is in collaboration with the Beijing Cultural Center and will ultimately be exhibited in a theater.
-->

---
layout: two-cols
---

# Exhibition Demo

<br/>

<img src="/cloudDemo.png" class="w-100 h-100">

::right::

<br/>
<br/>
<br/>

<img src="/foxDemo.png"  class="w-100 h-100 mt-1">

<!--
This slide showcases our expected goals. On the left, users can scan a marker on the ceiling with their phones to observe a changing cloud. The cloud will change color based on the color of the marker behind it. On the right, users can interact with a fox by scanning a marker on the ground. The fox will react differently based on changes in its surrounding environment.
-->

---
src: ./timeline.md
---

---
layout: two-cols
---

# Main Page

> User select the page they want to go to by clicking the button in the main page

* 🏃‍♂️ View by Motion Sensor
* 🖐️ Scale by Finger Touch
* 🔘 Click the Button to Redirect to the Page

::right::

<div class="w-full h-full flex justify-center items-center">
  <iframe src="https://cloud.lawted.tech" class="h-full w-2/3 rounded-xl"></iframe>
</div>

<!--
First up is the homepage. All the pages have been deployed to my personal website, cloud.lawted.tech. When you enter the homepage, you will see the model. By clicking on the corresponding model, you will be taken to the AR website. In the website, we have utilized the gyroscope to control the model. Currently, the model of the cloud is still being refined, so we have used a cube as a placeholder for now.
-->

---

<div class="grid grid-cols-4 gap-4">

<div class="col-span-3">

# Cloud Page

> Users scan the marker on the ceiling with their mobile phone to observe the cloud, and the cloud will change color according to the color behind the marker

<br/>

## ✅ Finished
* ☁️ Deploy the [Cloud Page](https://cloud.lawted.tech/cloud)
* 🎨 Track the Main Color of the Screen and Change the Color of the Cloud
* ⚙️ Orbit Control the Object and Scale by Finger Touch

## 🚧 In Progress
* <FileIconsVertexshader/> Use shader to implement the cloud effect (volume ray cast effect)

</div>

<div class="col-span-1 h-full flex justify-center items-center">
  <video src="/cloud-page.mp4" class="rounded-xl object-scale-down" controls autoplay loop></video>
</div>

</div>

<!--
In the video on the right, we can see how the cloud is currently being tracked through a marker. When the background color behind the cloud changes, the cloud's base color changes quickly in response. From different angles, you can observe different sides of the cloud, as if there is a real cloud floating in space.

Moving forward, I will utilize ray tracing algorithms to make more detailed adjustments to the cloud model, creating a more volumetric and soft appearance. Our goal is to create a realistic and immersive experience that allows users to feel as if they are truly interacting with a cloud in real life. We believe that by pushing the boundaries of what is possible with AR technology, we can create a new and exciting way for people to experience and appreciate art.
-->

---

<div class="grid grid-cols-4 gap-4">

<div class="col-span-3">

# Fox Page

> Users can observe the fox by scanning the signs on the ground, and change the fox's actions by talking and shouting.

<br/>

<div class="absolute right-80 top-60 flex">
<div class="flex flex-col justify-between h-50 mr-1">
  <h3>
    HIGH
  </h3>
  <h2 style="writing-mode: vertical-rl; transform: rotate(180deg)" >
    Volume
  </h2>
  <h3 >
    Low
  </h3>
</div>

<div class="flex flex-col border-light-500 border-2 rounded-lg justify-between my-1 ">

  <div class="bg-red-400 rounded-t-md h-20 text-center"> run </div>
  <div class="bg-green-400 h-15 text-center"> walk </div>
  <div class="bg-gray-400 rounded-b-md h-15 text-center p-1"> survey </div>


</div>
</div>


## ✅ Finished

* 🦊 Deploy the [Fox Page](https://cloud.lawted.tech/fox)
* 🔊 Detect the level of the surrounding environment volume
* 🎥 Animation will Change when Volume Meter Changes
* ⚙️ Orbit Control the Object and Scale by Finger Touch

## 🚧 In Progress
* <LogosTensorflow/> Use `tensorflow.js` to detect the voice by human
* 🎬 Create more animation for the fox

</div>


<div class="col-span-1 h-full flex justify-center items-center">
  <video src="/fox-page.mp4" class="rounded-xl object-scale-down" controls autoplay loop></video>
</div>

</div>

<!--
In the video on the right, we can see a fox turning its head on a marker. On the small box on the left side of the screen, the current surrounding volume is displayed. When I speak, the fox will walk, and when I shout, it will run. Currently, the interaction between the fox and the user is mainly based on the volume of the user's voice.

Moving forward, I will utilize TensorFlow.js to recognize the user's voice and enable the fox to make more diverse and responsive actions. Our goal is to create a more interactive and engaging experience for users, allowing them to feel a deeper connection with the AR art and the environment it creates.
-->

---
layout: quote
---

# "Thanks for your listening!"

<!--
In conclusion, I am very excited about the progress we have made so far with applying AR technology to art exhibition on mobile devices. By leveraging the latest advancements in AR, machine learning, and other cutting-edge technologies, we are creating a unique and immersive experience that allows users to interact with art in a whole new way.

Thanks for your listening
-->
