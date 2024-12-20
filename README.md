(#gemelo-digital-control-telemático-y-rv-generada-por-nerf-y-3dgs-en-tareas-de-rescate)

# DIGITAL TWIN, TELEMATIC CONTROL AND VR GENERATED BY NERF AND 3DGS IN RESCUE TASKS
<div align="justify">
In the digital age, digital twins have emerged as key tools for the simulation and real-time control of complex physical environments. This final degree project (TFG) presents an immersive telematic control system that combines digital twins with virtual reality (VR) in Unreal Engine, employing advanced technologies such as Neural Radiance Fields (NeRF) and 3D Gaussian Splatting (3DGS). The research demonstrates the feasibility of integrating these 3D reconstruction methods into rescue operations, providing an immersive and detailed visualization of the affected environment, facilitating a faster response and reducing the risk for rescue teams. The main contributions include the identification of optimal tools for the generation of 3D models compatible with the simulation of digital twins, the evaluation of robustness and deployment times in realistic scenarios, and the compatibility with the research lines in simulation and telematic control of the Robotics and Cybernetics Laboratory (ROBCIB) of the CAR ETSII UPM-CSIC. The combination of tools allows for effective deployment in approximately one and a half hours, demonstrating its applicability in simulated rescue situations.
</div>

&nbsp;
&nbsp;

<div align="center">

<img height="200" alt="(a) Thermal camera. 3DGS robustness tests. Images inside the Unreal Engine simulation" src="https://github.com/user-attachments/assets/5bf5a4e0-953b-40ab-a999-4aea5d00673a" >
<img height="200" alt="(a) Under the sea. 3DGS robustness tests. Images inside the Unreal Engine simulation" src="https://github.com/user-attachments/assets/109712de-76bb-47a6-86c7-bd6243763262" >
<img height="200" alt="(a) Smoke. 3DGS robustness tests. Images inside the Unreal Engine simulation" src="https://github.com/user-attachments/assets/f2a9ae73-9c2a-4e56-a747-35a7b3511757" >
<img height="200" alt="(a) Flowers (complex geometry). 3DGS robustness tests. Images within the Unreal Engine simulation" src="https://github.com/user-attachments/assets/36176a2e-84b2-448c-9952-6ba89b2c71c7" >

> 3DGS robustness tests[^2]. From left to right and top to bottom: thermal camera, underwater, smoke, flowers (complex geometry). Images inside the Unreal Engine simulation. _Source: Author_

&nbsp;
&nbsp;

![Deployment of technology in a simulated rescue situation](https://github.com/user-attachments/assets/1a185adc-16fa-4f26-bab2-833bc96975ab)

> Deployment of technology in a simulated rescue situation. _Source: Author_

</div>

&nbsp;
&nbsp;

## About this repository
<div align="justify">
  
In this repository you will find:
- The source code of the nodes and the launcher with the ROS parameters necessary for communication between the robot and Unreal Engine.
- The complete Unreal Engine 5.2 project used for the development of the work, including the plugins with the modifications indicated in the report.
- The installation and use manuals for the tools used.
- The compilation of basic ROS concepts and commands necessary for the project.
</div>

## Accessible information
<div align="justify">
The work report can be consulted in the UPM Digital Archive.

- Link: [https://oa.upm.es/83722/](https://oa.upm.es/83722/)

Additionally, the following YouTube channel is available where you can find the first tests carried out with instant-ngp, the robustness tests of the capacity to generate 3D models for environments considered difficult and the demonstration video of the deployment of the technology.

- Youtube Channel: [https://www.youtube.com/watch?v=sjYeZrFqgSc&t](https://www.youtube.com/watch?v=sjYeZrFqgSc&t)

The list of videos found on the YouTube channel is as follows:
1. Demonstration of the complete workflow
2. instant-ngp - Yellow Flowers Training
3. 3DGS Robustness Tests - Environments with repetitive elements
4. 3DGS Robustness Tests - Small objects
5. 3DGS Robustness Tests - Elements with complex geometries
6. 3DGS Robustness Tests - Scenes with smoke or fog
7. 3DGS Robustness Tests - Night scenes
8. 3DGS Robustness Tests - Thermal camera recordings
9. 3DGS Robustness Tests - Scenes with reflections and refraction
</div>

## General description
<div align="justify">
In the digital era, digital twins have emerged as fundamental tools for the simulation and real-time control of complex physical environments. This work presents the development of an immersive telematic control system that combines digital twin technology with virtual reality (VR), generated from Neural Radiance Fields (NeRF) and subsequent developments derived from it such as 3D Gaussian Splatting (3DGS).

To illustrate the starting point, Figure 0.1 presents a typical training scenario for Digital Twins (0.1a) and the state of the art in teleoperation of robotic systems with virtual reality interfaces in the Robotics and Cybernetics Laboratory (ROBCIB) of CAR ETSII - UPM (0.1b); and Figure 0.2 presents examples of 3D models of complex physical environments in which it is proposed to deploy said digital twins.

&nbsp;
&nbsp;

</div>
<div align="center">

<img height="150" alt="Example (a) of Digital Twins in artificial or unrealistic environments" src="https://github.com/user-attachments/assets/751acb4a-73df-4233-9bd6-b63de7f39f2c" >
<img height="150" alt="Example (b) of Digital Twins in artificial or unrealistic environments" src="https://github.com/user-attachments/assets/f53dd621-1235-438d-bf9e-e698f8c36276" >

> Figures 0.1a and 0.1b. Examples of Digital Twins in artificial or unrealistic environments. _Sources:_ [^3] y [^4].

&nbsp;
&nbsp;

<img height="300" alt="Examples of 3D models of complex environments generated with 3DGS" src="https://github.com/user-attachments/assets/8b7f329f-a1af-4639-8341-a7336d56de95" >

> Figure 0.2: Examples of 3D models of complex environments generated with 3DGS. _Sources:_ [^2]

&nbsp;
&nbsp;

</div>
<div align="justify">

This research seeks to demonstrate that it is possible to integrate these 3D model reconstruction technologies with rescue operations in emergency situations, providing operators with an immersive and detailed visualization of the affected environment.

The precise and realistic reconstruction of three-dimensional environments from two-dimensional images in which the digital twins of the deployed robots can operate also allows the simulation of possible catastrophe scenarios.

In this way, it not only facilitates a faster and more effective response, but also reduces the risk for rescue teams.

The main contributions of this project are the following:
1. The optimal combination of tools to obtain a 3D model compatible with the simulation of the digital twins of the robots.
2. The robustness and deployment time of the technology in realistic application situations.
3. Compatibility with the current lines of research of the Robotics and Cybernetics Laboratory (ROBCIB) of the CAR ETSII UPM-CSIC, in particular the simulation and telematic control of robots through the use of virtual reality for closer and safer collaboration between operators and robots.

The combination of the tools used in this project allows the deployment of the technology in approximately one and a half hours for a simulated rescue situation.

After discarding instant-ngp[^5] and Unity due to incompatibilities, the tools compiled in the list below have been chosen. Figure 0.3 shows the complete workflow diagram of these tools, and then Table 0.1 shows the times used for their deployment.

- FFmpeg[^6], for preprocessing, and COLMAP[^7] with the addition of hloc[^8], for obtaining the photogrammetry.
- Splatfacto[^9] (NerfStudio[^9] environment method for 3DGS[^2]) and volinga-model[^10], for generating the 3D model of the scene.
- Volinga Suite[^10], for compatibility with Unreal Engine (UE).
- UE together with the Volinga plugin[^10], for its representation in a virtual reality environment compatible with the simulation of the digital twins of the robots.
- Rosbridge[^11] and ROSIntegration[^12], for compatibility with current lines of research that use the ROS standard.
</div>
<div align="center">

&nbsp;
&nbsp;

<img alt="Complete workflow" src="https://github.com/user-attachments/assets/7f7ed627-fc66-483e-a8ea-2afcc8328fd5" >

> Figure 0.3: Complete workflow. _Source: own elaboration_

&nbsp;
&nbsp;

<img height="300" alt="Full Workflow Deployment Time Table" src="https://github.com/user-attachments/assets/b4998254-9a7f-4310-8a9f-b1108d60f0b7" >

> Table 0.1: Table of deployment times for the complete workflow. _Source: Own elaboration_

</div>
<div align="justify">

&nbsp;
&nbsp;

The appearance of the technology deployed during the demonstration can be seen in the images in Figure 0.4.
</div>
<div align="center">

&nbsp;
&nbsp;

<img alt="Full workflow demonstration" src="https://github.com/user-attachments/assets/4ff0cf6a-3136-4187-ab96-527165159d97" >

> Figure 0.4: Demonstration of the complete workflow. _Source: own elaboration_

&nbsp;
&nbsp;

</div>

## Keywords
<div align="justify">
Digital Twin, telematic control, immersive simulation, NeRF, Gaussian Splatting, Unreal Engine, virtual reality for rescues.
</div>

## References
[^1]: Mildenhall, B. et al. (2020). _NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis_. En: _ECCV 2020 Oral_. url: [https://www.matthewtancik.com/nerf](https://www.matthewtancik.com/nerf)
[^2]: Kerbl, B., Kopanas, G., Leimk¨uhler, T. y Drettakis, G. (jul. de 2023). _3D Gaussian Splatting for Real-Time Radiance Field Rendering_. En: _ACM Transactions on Graphics 42.4_. url: [https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/).
[^3]: Rudin, N., Hoeller, D., Reist, P. y Hutter, M. (2021). _Learning to Walk in Minutes Using Massively Parallel Deep Reinforcement Learning_. En: _ArXiv abs/2109.11978_. url: [https://api.semanticscholar.org/CorpusID:237635100](https://api.semanticscholar.org/CorpusID:237635100).
[^4]: Cruz Ulloa, C. (mar. de 2024). _Quadrupedal Robots in Search and Rescue: Perception and Teleoperation_. doi: 10.20868/UPM.thesis.81769. url: [https://oa.upm.es/81769/](https://oa.upm.es/81769/).
[^5]: Müller, T., Evans, A., Schied, C. y Keller, A. (jul. de 2022). _Instant Neural Graphics Primitives with a Multiresolution Hash Encoding_. En: _ACM Trans. Graph. 41.4_, 102:1-102:15. doi: 10.1145/3528223.3530127. url: [https://doi.org/10.1145/3528223.3530127](https://doi.org/10.1145/3528223.3530127) y [https://nvlabs.github.io/instant-ngp/](https://nvlabs.github.io/instant-ngp/).
[^6]: Tomar, S. (2006). _Converting video formats with FFmpeg_. En: _Linux Journal 2006.146, pág. 10_. url: [https://www.ffmpeg.org/](https://www.ffmpeg.org/)
[^7]: Schönberger, J. L., Zheng, E., Pollefeys, M. y Frahm, J.-M. (2016). _Pixelwise View Selection for Unstructured Multi-View Stereo_. En: _European Conference on Computer Vision (ECCV)_. url: [https://colmap.github.io/](https://colmap.github.io/)
[^8]: Sarlin, P.-E., Cadena, C., Siegwart, R. y Dymczyk, M. (2019). _From Coarse to Fine: Robust Hierarchical Localization at Large Scale_. En: _CVPR_. url: [https://github.com/cvg/Hierarchical-Localization](https://github.com/cvg/Hierarchical-Localization)
[^9]: Tancik, M. et al. (2023). _Nerfstudio: A Modular Framework for Neural Radiance Field Development_. En: _ACM SIGGRAPH 2023 Conference Proceedings. SIGGRAPH ’23_. url: [https://docs.nerf.studio/](https://docs.nerf.studio/)
[^10]: Volinga development team (2023). _Volinga Suite, volinga-model and Volinga plugin_. url: [https://volinga.ai/](https://volinga.ai/) y [https://github.com/Volinga/volinga-model](https://github.com/Volinga/volinga-model)
[^11]: Crick, C., Jay, G., Osentoski, S., Pitzer, B. y Jenkins, O. C. (2011). _ROSbridge: ROS for Non-ROS Users_. En: _Proceedings of the Robotics Systems Science and Systems Conference (RSS)_. url: [http://rosbridge.org](http://rosbridge.org).
[^12]: Schmeisser, M. y Suero, M. (2018). _ROSIntegration: Connecting Unreal Engine with ROS for Realistic Simulations_. En: _Proceedings of the IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)_. url: [https://github.com/code-iai/ROSIntegration](https://github.com/code-iai/ROSIntegration).
