---
layout: post
title: Hatil Virtual Store
subtitle: 'HATIL Complex Ltd. , Bangladesh'
categories:
  - game-xr
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

## Project Description

Using **Unity3D**, HATIL Virtual Store was designed and developed as a **“Virtual Store”** solution, essentially a store inside a store. HATIL installed large screens through projectors, TV displays, and similar systems inside their retail outlets. On these screens, customers could browse HATIL’s full range of furniture, including product variations, in interactive 3D and virtual reality.

![Hvs_Store_1](/assets/img/hatil_Article.jpg)

Customers could change fabric and material combinations, explore furniture in highly detailed 3D, and view products up close through a virtual reality experience. The platform also included a **Room Planner** tool, where sales agents could recreate customer room layouts and test different furniture combinations. The Room Planner supported different room sizes, customizable walls and floors, doors, windows, accessories, and VR viewing.

![Hvs_Store_2](/assets/img/hatil_Article_2.jpg)

The software ecosystem also included backend and designer-facing tools for HATIL’s internal teams. Designers could use the **Designer Toolkit** to select fabric combinations and prepare furniture sets that customers would later see inside the Gallery space of the Virtual Store.

The Virtual Store eventually ran in **20+ stores across Bangladesh and India**. In some stores, up to **50% of monthly sales** came through this setup. The platform helped HATIL reduce dependency on large physical retail space while giving customers access to a wider range of furniture options and a more informed buying experience.

![Hvs_Store_3](/assets/img/hatil_Article_3.jpg)

## My Contribution & Technical Challenges

I was heavily involved in the **design, development, and deployment** of the application. Since we were working in a startup environment, the project required taking initiative across multiple parts of the software stack to make the vision possible: a centrally controlled virtual retail store that could be deployed across multiple physical locations, updated remotely, and authenticated for licensed use at a national scale.

One of the biggest challenges was that there were very few examples of a product like this at the time. We had to take a leap into an unfamiliar space and figure out how to turn the idea of a scalable virtual retail store into a working product. Since our startup team had experience shipping smaller Unity3D projects, we used **Unity3D** as the foundation and built additional systems on top of it, including **web-service integration, dynamic content loading, modular installation, and runtime update workflows**.

I was directly involved in implementing the **UI, application flow, product browsing experience, and customization logic**. I actively contributed to the design and development of the **runtime game-asset database system**, helping define how furniture assets, material options, and customization attributes could be updated dynamically without requiring a full application rebuild.

I was also involved in the **3D asset-generation pipeline** needed to bring HATIL’s retail furniture catalog into the Virtual Store. The furniture models were created through 3D scanning, but a major challenge was supporting fabric and texture customization while still preserving the real-world details of each product. To solve this, we used multiple UV channels: furniture-specific details such as bumps, normals, and surface characteristics were baked into a secondary UV channel, while the primary UV channel was used for tileable fabric textures.

To support realistic customization, available fabrics were scanned and converted into digital texture sets. These textures were then projected onto the furniture meshes using a triplanar-style projection approach, allowing fabric changes to be applied dynamically while still preserving the scanned model details. The combination of scanned geometry, baked detail maps, and customizable fabric textures helped produce furniture models that closely resembled their real-life counterparts.

I also contributed to the **Room Planner** and the virtual reality environment that complemented the default retail browsing experience. This included supporting interactive room customization workflows and helping users visualize furniture arrangements in a more immersive way.

Another important part of my work was developing **Unity3D editor tools** and **content-management workflows** that could be handed over to non-technical users. This allowed HATIL’s internal teams to maintain product content, update furniture sets, and manage design combinations without requiring developer involvement for every content change.

A major contribution of mine was building the **distribution, update, licensing, and authentication system**. I developed a **C#/.NET launcher application** that used **AWS S3** to download the Unity application in split parts, update itself, and notify users when new updates were available. This helped distribute large application binaries and asset packages more reliably across retail locations.

I also implemented **in-application authentication, hardware-bound licensing, and anti-tampering mechanisms** using **hashing and cryptographic checks** to protect the software from unauthorized use or modification. These systems were important for deploying and maintaining the application across multiple retail locations while keeping control over licensing, updates, and content distribution.

<iframe width="560" height="315" src="https://www.youtube.com/embed/D4uAItpOvT0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
