---
theme: default
background: https://massivepixel.io/wp-content/uploads/2021/10/virtual-dom-hero-header-scaled-1.jpg
class: text-center
highlighter: shiki
lineNumbers: false
drawings:
  persist: false
transition: slide-left
title: React Server Components
layout: cover
---

# React Server Components

<span class="author">
    Shaswat Prabhat | <carbon-logo-github/> ShaswatPrabhat | <carbon-logo-twitter/>@ShaswatPrabhat 
</span>


<style>
p{
  font-size:24px;
}
.author {
  font-size: 16px;
  margin-top: 10%;
}
</style>


---
transition: slide-left
layout: cover
---

# Story-time

<v-click>

## A restaurant experience

</v-click>
---
transition: slide-left
layout: two-cols
---

<v-click>

# Experience 1

</v-click>


<v-click>

1. Arrive at table
2. Place the order

</v-click>

<v-click>

3. Watch the Chef cook the food  
</v-click>

<v-click>

  3a. Watch the Chef peel the onion ...<br/>
</v-click>
<v-click>

  3b. Watch the Chef dice the carrot ...<br/>
</v-click>
<v-click>

   <span class="animate-ping" style="font-size:36px">...</span>

</v-click>

<v-click>

4. Get served food

</v-click>



::right::

<v-click>

# Experience 2

</v-click>


<v-click>

1. Arrive at table
2. Place the order

</v-click>

<v-click>

3. Scroll a feed on your phone   

</v-click>

<v-click>

3a. Switch apps ...<br/>

</v-click>

<v-click>

3b. Repeat 3 ...<br/>

</v-click>

<v-click>

<span class="animate-ping" style="font-size:36px">...</span>

</v-click>

<v-click>

4. Get served food

</v-click>


---
transition: slide-left
layout: center
---

# What if ?

<v-click>

1. Arrive at table
2. Place the order

</v-click>

<v-click>

3. Watch the chef prepare your food

</v-click>

<v-click>

3a. A fast shiny spectacle...<br/>

</v-click>

<v-click>

3b. Hypnotized by the speed!<br/>

</v-click>

<v-click>

<span class="animate-ping" style="font-size:36px">...</span>

</v-click>

<v-click>

4. Get served food

</v-click>


---
transition: slide-left
layout: cover
---
# Welcome !

---
layout: two-cols
transition: slide-left
---

# Aims
What this talk will cover:
<br/>
<v-click>

### 1. Mental Model 
<br/>
<br/>
</v-click>
<v-click>

### 2. Motivation
<br/>
<br/>
</v-click>
<v-click>

### 3. Re-understand "Server"
<br/>
<br/>
</v-click>

::right::

<v-click>

# Anti-Aims
What this talk will not cover:
<br/>
</v-click>
<v-click>

### 1. Comparison of landscape
<br/>
<br/>
</v-click>
<v-click>

### 2.Infrastructure and Setup
<br/>
<br/>
</v-click>
<v-click>

### 3. Framework implementations
<br/>
<br/>
</v-click>

---
transition: slide-left
---

# A super quick vocabulary check
* <carbon-logo-react /> React - A client-side rendered library for components based Web Application 
* <carbon-connection-two-way /> State - Intelligent variables
* <carbon-laptop /> CSR - Client side Rendering
* <carbon-bare-metal-server /> SSR - Server side Rendering

---
transition: slide-left
layout: fact
---

# Network Chasm and attention deficit
Lesser time available to grab user's attention

---
transition: slide-left
---

# Path to Server Components - I
<img 
height="640"
width="640"
src="https://nextjs.org/_next/image?url=%2Fdocs%2Fdark%2Fthinking-in-server-components.png&w=3840&q=75&dpl=dpl_9ban2Vw5rf63ZAqeHHQT5v4nYHuz">
* Page divided into Interactive and non-interactive components
* What can we do after having segregated this
<p style="font-size:12px; color: aqua"><mdi-alert-box /> Several ideas span from the above - including Micro front-ends, Islands Architecture etc</p>
---
transition: slide-left
---

# Path to Server Components - II
<img height="600"
width="600"
src="https://s42821.pcdn.co/wp-content/uploads/2022/07/Image-AWS-Edge-Network@2x.png">
* Rise of "Edge runtimes" - deploy closer to the user
* The network chasm between Client and Server is decreasing
<p style="font-size:12px; color: aqua"><mdi-alert-box /> Almost all layers of the OSI stack are becoming faster and scalabale.</p>
---
transition: slide-left
---

# Path to Server Components - III
* <mdi-connection /> The database, services and browsers are quickly becoming more connected
* <mdi-server-remove /> While Client-Server Architecture is still relevant, we might need to unlearn some of the concepts
* <mdi-speedometer /> Our applications need to be ready to deliver content at scale and at speed
* <mdi-transit-connection-variant /> All of these ideas converge into RSC
---
transition: slide-left
layout: fact
---

# Parsing the RFC
Some phrases from the RFC and their intent

---
transition: slide-left
layout: statement
---
# "Spanning the client and the server"

---
transition: slide-left
layout: statement
---
# "Incrementally Stream rendered data"

---
transition: slide-left
layout: statement
---
# "Easier to fetch data"






