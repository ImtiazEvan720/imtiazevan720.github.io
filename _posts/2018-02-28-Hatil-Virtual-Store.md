---
layout: post
title: Hatil Virtual Store
subtitle: 'HATIL Complex Ltd. , Bangladesh'
tags:
  - Unity3d
  - 'C#'
  - Oculus Rift
  - VR
comments: false
published: true
thumbnail-img: /assets/img/Hatil-Furniture-Thumb.jpg
cover-img: /assets/img/hvs.jpeg
---

Hatil, Bangladesh’s largest furniture brand was facing a challenge with increasing rent costs of retail spaces. Especially in city centers, where the majority of Hatil’s customers prefer shopping, Hatil was not being able to display their full range of furniture. At any given point Hatil has an inventory close to 1000. And if you add fabric and accessories varieties, then there is literally thousands of options for customers.


**My Role :** _Core Developer_ 

**Tech Stack :** _C#, Unity3d, PHP/Laravel_ 

**Platform :**_Windows, Oculus Rift, HTC Vive_

**Project Description :**

Using **Unity3D**, HATIL Virtual Store was designed and developed as a **“Virtual Store”** solution, essentially a store inside a store. HATIL started setting up large screens through projectors, TV screens, and similar display systems inside their retail outlets. On these screens, customers could browse HATIL’s full range of furniture, including variations, in interactive 3D and virtual reality.

One of the biggest challenges was that there were very few examples of a product like this at the time. We had to take a leap into an unfamiliar space and figure out how to turn the idea of a scalable virtual retail store into a working product. Since our startup team had experience shipping smaller Unity3D projects, we used Unity3D as the foundation and built additional systems on top of it, **including web-service integration, dynamic content loading, modular installation, and runtime update workflows.**

![Hvs_Store_1](/assets/img/hatil_Article.jpg)

I was heavily involved in the **design, development, and deployment** of the application. Since we were working in a startup environment, the project required taking initiative across multiple parts of the software stack to make the vision possible: a **centrally controlled** virtual retail store that could be deployed across multiple physical locations, updated remotely, and authenticated for licensed use at a national scale.

Customers had the ability to change fabric and material combinations for furniture and browse the full HATIL collection in highly detailed 3D. They could also view furniture up close through a virtual reality experience. I was directly involved in implementing the **UI, application flow, product browsing experience, and customization logic**. I actively contributed to the design and development of the runtime game-asset database system, helping define how furniture assets, material options, and customization attributes could be updated dynamically without requiring a full application rebuild.

![Hvs_Store_2](/assets/img/hatil_Article_2.jpg)

Quite often, customers came to HATIL stores with their room or apartment layouts, looking for the best suggestions for their interiors. To support this, we built a Room Planner tool where sales agents could quickly recreate customer rooms and test furniture combinations. The Room Planner supported different room types and sizes, customizable walls and floors, doors, windows, accessories, and VR viewing. I also contributed to the virtual reality environment that complemented the default retail browsing experience.

The software ecosystem also included an easy-to-use backend and designer workflow for HATIL’s internal teams. Designers could use the Designer Toolkit to select fabric combinations and prepare furniture sets that customers would later see inside the Gallery space of the Virtual Store. I worked on Unity3D **editor tools and content-management** workflows that could be handed over to non-technical users, allowing the business team to maintain and update product content without requiring developer involvement for every change.

![Hvs_Store_3](/assets/img/hatil_Article_3.jpg)

A major contribution of mine was building the **distribution, update, licensing, and authentication** system. I developed a **C#/.NET** launcher application that used **AWS S3** to download the Unity application in split parts, update itself, and notify users when new updates were available. This helped us distribute large application binaries and asset packages more reliably across retail locations. I also implemented **in-application authentication, hardware-bound licensing, and anti-tampering** mechanisms using **hashing and cryptographic** checks to protect the software from unauthorized use or modification.

The Virtual Store eventually ran in **10+ stores across Bangladesh and India**. In some stores, up to **50% of monthly** sales came through this setup. The platform helped HATIL reduce dependency on large physical retail space while giving customers access to a wider range of furniture options and a more informed buying experience. With the success of the first pilot deployments, HATIL prepared to scale the system further across additional retail locations.

<iframe width="560" height="315" src="https://www.youtube.com/embed/D4uAItpOvT0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
