# Maya_Archeology_Web

## Links

[E4E Maya Archeology Subteam](https://e4e.ucsd.edu/maya-archaeology)

Early draft of my research paper (Will be released when published or added to E4E wiki)

[Working version of the project](https://fabricant.ucsd.edu:3443/) (Currently offline)

## Overview

<p align="center"> <img src="/images/top.png" width="600"/> </p>
<br />

Engineers for Exploration is a research-heavy program stationed at the University of California, San Diego. One of the team's projects is Maya Archeology, a group responsible for digitally preserving sensitive archeological sites in Central America by scanning them, and converting them into 3D data. Maya Archeology is a large project consisting of a few subteams, specifically the VR Visualization subteam which focuses on cleaning and visualizing this data. Part of my requirement to graduate with departmental honors as an undergrad at UCSD was to complete a research project, which was my original motivation for approaching the team. The idea was that I would provide E4E with a complete project to help visualize their findings, in exchange for performing research with this project and their resources. My responsibility on this subteam was to develop a web-based VR program capable of navigating and exploring the archeological sites. While this was started and completed as a solo project, I used assets provided by the program, and had guidance from senior members and my mentor.
  
I had two major responsibilities on the project: complete the navigable 3D environennt, and conduct original research in the process. Finishing development of the program itself was my first priority, the final working draft coming to completion early Summer 2022. While in the process of development, I came up with a few techniques that take advantage of the GPU-heavy hardware of VR devices to load 3D textures using multithreading rather than JavaScript's traditional single-threaded execution. This became the focus of my research paper, which is listed in the links above.
  
This is the project I have put the most effort into by far. I believe myself to be most proficient at projects that are computationally or mathematically heavy, which the Maya Web project clearly displays. It also demonstrates that I am capable of supporting a full-stack Web project through its entire life cycle - from scratch to a finished project.

<br />

> NOTE: This repository contains *only* the code I wrote (in *src*) and the code required to run BabylonJS (in *node_modules*, added by running `npm run build` after downloading the project). The required models and textures belong to E4E and are excluded - therefore the program won't run properly without erroring

<br />
  
The entrypoint for the application is via *app.ts*, though most of the work is done in the *Environment.ts* file. Again, the main purpose of this repository is to demonstrate my coding style, not to provide a working version of the project. This is a Typescript project that heavily uses the [BabylonJS](https://www.babylonjs.com/) Engine, run with [WebPack-Dev-Server](https://webpack.js.org/configuration/dev-server/) and Docker.

<br />

<p align="center"> <img src="/images/example.gif" width="500"/> </p>

> An example of what a high-quality early build looks like in VR

<br />

<p align="center"> <img src="/images/frontend.png" width="500"/> </p>

> The research and computation  took head on this project - while there are quality of life additions to the project (like a loading screen and a larger "enter VR" button) - the frontend wasn't a focus even towards the end of the project's development.