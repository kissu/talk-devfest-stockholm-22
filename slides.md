---
title: 'Quickstart on 3D principles + MACHINES 🤖'
theme: seriph

# fonts:
  # sans: '"DM Sans"'

download: true
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://images.unsplash.com/photo-1655635643532-fa9ba2648cbe?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2832&q=80

# photo from: https://unsplash.com/photos/qhhp1LwvPSI

drawings:
  enabled: dev
# Photo by <a href="https://unsplash.com/@heytowner?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">JOHN TOWNER</a> on <a href="https://unsplash.com/s/photos/mountains?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>

# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
colorSchema: 'dark'
---

# Tasty 3D and crunchy robots 🤖

They are stealing our jobs!

<!-- This is a page note btw -->

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171331451-8e66c500-b7d1-48ad-a222-08a5ba71a3d5.svg
---

# Can we have some 3D please? 🤩

<!--
for 3D on the Web, we use WebGL, it's fast because it's using the GPU so that our users don't wait too long

we can generate millions of polygons in just a matter of milliseconds

we will then be able to get a nice image + it's a Web standard

we have some documentation, a standard etc...let's see how amazing it is!

let's see how to make a nice cube thanks to WebGL

[presentation of the hardcore codebase 😱]

not that amazing huh? not gonna write that kind of code daily unfortunately 😪
-->

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171331451-8e66c500-b7d1-48ad-a222-08a5ba71a3d5.svg
---

<h2 class="mb-8 !text-4xl">Why would somebody use ThreeJS? ✨</h2>

<div class="text-left">
<v-clicks>

- a lot is available out of the box
- no need to be an expert in 3D to have fun
- reduces the amount of code to write by a lot
- documentation and examples are amazing too: https://threejs.org/

</v-clicks>
</div>

<!--
geometries, lights, materials, etc... are available out of the box

3D can have quite some requirement regarding the physics, maths, what is a quaternion, how to make a matrix rotation etc...most of it is not needed when working with ThreeJS

let's see how to write the same with ThreeJS

[demo of the simple geometry /02 + proper spinning cube]

as you can see, the difference is quite substantial and far more readable (especially if you're used of writting JS)

far better than to read 300 pages of an old book with just text
-->

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171331451-8e66c500-b7d1-48ad-a222-08a5ba71a3d5.svg
---

<h2 class="mb-8 !text-4xl">Some cool projects 🚀</h2>

<div class="text-left pl-36">

[NuxtJS, meta-framework for VueJS](https://v3.nuxtjs.org/)

[Simple and cool animation for any portfolio](https://www.craftz.dog/)

[Realistic render of a rental house](https://twitter.com/rocha_ycaro/status/1529205485731299335/photo/1)

[Deus Ex game, weapon customization](https://infinitemirai.files.wordpress.com/2015/08/vlcsnap-00025.png)

[Pinball based on a french train company](http://letsplay.ouigo.com/)

[Bruno Simon's resume](https://bruno-simon.com/)

[Want to design your own iPhone?](https://neal.fun/design-the-next-iphone/)

</div>

<!--
I already have the links opened in my group tabs
-->

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171331451-8e66c500-b7d1-48ad-a222-08a5ba71a3d5.svg
---

<h2 class="mb-8 !text-4xl">What do we need exactly?</h2>

<div class="flex">
<img class="h-84" src="https://threejs.org/manual/resources/images/threejs-1cube-with-directionallight.svg" />

<div class="text-left">
<v-clicks>

- all the fundamentals are available [here](https://threejs.org/manual/#en/fundamentals)
- renderer, wrapping all the other parts
- scene, the tree of our objects
- mesh 👉 geometry + material
- geometry, the shape of our object
- material, the surface properties
- light, so that we see our objects
- texture (optional)

</v-clicks>
</div>

</div>

<style>
.slidev-layout ul {
  list-style-type: initial
}
</style>

<!--
a renderer receives a scene and a camera to render all of them down the tree

the scene contains lights, geometries, cameras, materials, etc... this hierarchy is containing all
the children and the info about where they are aiming, where they appear. think of it as a scene in a film.

the mesh helps us know the position and orientation of each cube

the geometry will indicate us if it's a sphere, cube, taco, dog, building of a conference etc...

a material can be shiny, rough, transparent, etc... it's the surface of our object and is basically
represented by any specifics that you can find in real world

a light is usually needed especially if the object is not glowing by itself

a texture is usually an image or a canvas, for example some patterns of grass/dirt/rock holes

all of those have a lot of variants with customizable properties and all of them are available thanks to ThreeJS
-->

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171331451-8e66c500-b7d1-48ad-a222-08a5ba71a3d5.svg
---

<img class="mx-auto h-104" src="https://threejs.org/manual/resources/images/threejs-structure.svg" />

<div class="mt-8">
<v-clicks>

- When do we start?! Any requirements...?

</v-clicks>
</div>

<!--
understands the basics of JS (loops, variables)

being able to understand some concepts like aliasing, 3D space and how to navigate there

basics in Maths: Pi, cosinus/sinus

some hardware/gaming knowledge is optional but it may be handy to understand how to optimize the code
and what is happening internally

[let's go back to some code again and inspect the cube + a fancy GALAXY 🌌]
-->

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171331451-8e66c500-b7d1-48ad-a222-08a5ba71a3d5.svg
---

## What about more complex objects? 🤔

<iframe class="mx-auto mt-12" width="560" height="315" src="https://www.youtube-nocookie.com/embed/v0oIFf-NDww" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<!--
[show the map] quite a lot of things happening here, right?

it was some promotion for a VueJS conference that I like!

achieving this kind of video with just ThreeJS would take quite some time huh?

[introduction to Blender]
-->

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171334746-70ecbd5d-5acd-47d1-977a-062762ce7e95.svg
---

# Is it usable in ThreeJS?

### Of course it is, let's import our bike into a webpage! 🚲🌪️

<!--
[present troisJS page + whole 3 branches]
-->

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171334746-70ecbd5d-5acd-47d1-977a-062762ce7e95.svg
---

## You want more/where to learn? 🤯

<div class="pt-12 text-left">

- Bruno Simon with [three.js journey](https://threejs-journey.com/)
- Andrew Price aka "Blender Guru" with [his Donut playlist](https://youtu.be/OqMLfMXVhhI?list=PLjEaoINr3zgFX8ZsChQVQsuDSjEqdWMAD&t=1418)
- Roman Klčo aka Polygon Runway with [his course](https://polygonrunway.com/courses) + [YouTube channel](https://www.youtube.com/c/PolygonRunway/featured)

</div>

<!--
we do have custom shaders: https://threejs.org/examples/?q=shaders#webgl_shaders_ocean
-->

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171334746-70ecbd5d-5acd-47d1-977a-062762ce7e95.svg
---

## What about the ROBOTS?? 🤯🤖

<div class="mt-8 text-left">
<v-clicks>

- DALL-E 2.0
- Midjourney
- Stable Diffusion
- Now...? DREAMFUSION!

</v-clicks>
</div>

<!--
what do you think about that? will the robots get us all? 🤖🤖🤖
-->

---
layout: cover
preload: false
background: https://user-images.githubusercontent.com/5133074/171334746-70ecbd5d-5acd-47d1-977a-062762ce7e95.svg
---

<div class="absolute text-left top-12 left-14">
  <!-- <h2 class="!text-white underline decoration-wavy decoration-1 underline-offset-4 underline-grey-100">Your speaker</h2> -->

  <h3 class="mt-2">Konstantin BIFERT aka <span class="italic">kissu</span>
</h3>
</div>

<div class="flex mt-0">
  <img v-motion :initial="{ x: -200, y: 0, scale: 1, rotate: 0 }" :enter="final"
    class="w-64 h-64 rounded-lg" src="https://avatars.githubusercontent.com/u/5133074?v=4"
    alt="photo of konstantin" />

  <section class="ml-6 text-left">
    <p class="!m-0">
      <logos-vue/> Frontend Consultant <a href="https://twitter.com/passionpeopleNL">@passionpeopleNL</a> 🇳🇱
    </p>
    <p class="my-2">
      <logos-nuxt-icon class="inline h-6" />
      <a href="https://nuxtjs.org/teams" class="ml-2">Nuxt.js Ambassador</a>
    </p>
    <p class="my-2">
      <logos-stackoverflow-icon class="inline mr-2" />
      <a href="https://stackoverflow.com/users/8816585/kissu">Stackoverflow daily helper</a>
      <p>🎥  Launched a YouTube channel 👉 <a href="https://kissu.video" target="_blank" class="font-bold text-transparent bg-clip-text bg-gradient-to-tl from-orange-400 to-pink-500" alt="konstantin's YouTube channel">www.kissu.video</a></p>
      <p><logos-twitter class="h-4" /> Tweet'ing about cool stuff 👉 <a href="https://twitter.com/kissu_io" target="_blank" class="font-bold text-transparent bg-clip-text bg-gradient-to-tl from-blue-400 to-teal-500" alt="konstantin's twitter">@kissu_io</a></p>
      <p>✒️ Blogging really soon at 👉 <a href="https://kissu.io/" target="_blank" class="font-bold text-transparent bg-clip-text bg-gradient-to-tl from-emerald-400 to-green-500" alt="konstantin's twitter">kissu.io</a></p>
      <p>✨ I do enjoy mech keyboards, gaming, tech and DIY</p>
    </p>
  </section>
</div>

<script setup lang="ts">
  const final = {
    x: 0,
    y: 0,
    scale: 1,
    transition: {
      type: 'spring',
      damping: 10,
      stiffness: 20,
      mass: 2
    }
  }
  const melon = {
    x: 50,
    y: -50,
    rotate: 0,
    scale: 1,
    transition: {
      type: 'spring',
      damping: 10,
      stiffness: 20,
      mass: 2
    }
  }
</script>
