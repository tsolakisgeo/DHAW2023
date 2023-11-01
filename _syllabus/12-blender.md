---
class: 12
day: Thursday, November 2
title: 'Blender'
tags: 
---

## Assignment due: 
- Create two 3D models of interesting objects in Agisoft Metashape and upload them on Sketchfab. Put the link to your model on Canvas.

## Before Class 
- Download [Blender](https://www.blender.org/download/)

## Readings 
- Petras, E. (2021) Creating a 3D Map of an Archaeological Site in Blender. Available [here](https://sites.temple.edu/tudsc/2021/04/03/creating-a-3d-map-of-an-archaeological-site-in-blender/).
- Porter, S. (2022) Mixing things up in Three Dimensions: The Many Uses of Blender in Archaeology. Available [here](https://www.cambridge.org/core/blog/2022/10/26/mixing-things-up-in-three-dimensions-the-many-uses-of-blender-in-archaeology/).
- Košťál, N. (2019) Archaeology for 3D Modelling. Available [here](https://www.youtube.com/watch?v=bwMTTJogurE).

## Notes 

### Interface
[3D viewport](https://docs.blender.org/manual/en/latest/editors/3dview/index.html)

[Topbar](https://docs.blender.org/manual/en/latest/interface/window_system/topbar.html#)

[Menus](https://docs.blender.org/manual/en/latest/interface/window_system/topbar.html#menus)

![Menus]https://docs.blender.org/manual/en/latest/_images/interface_window-system_topbar_menus.png

[Workspaces](https://docs.blender.org/manual/en/latest/interface/window_system/topbar.html#workspaces)

![Workspaces]https://docs.blender.org/manual/en/latest/_images/interface_window-system_topbar_workspaces.png

### Blender shortcuts
- Shift + A: Add
- Tab: Swift between Object Mode and Edit Mode
- Shift + R: Repeat

### Creating a 3D model of Crete

##### QGIS
- First, you have to export two images from QGIS. Select a layer with elevation data and another with 
- Project -> Import/Export -> Export map to image (choose 1200 dpi)

##### Open Blender
  - Select and delete the cube
  - Select and delete the light
  - Shift + A -> Mesh -> Plane
- Go to Edit Mode
  - Right click on the place and Subdivide
  - Repeat (several times) with Shift + R
- Return to Object mode
- Modifier (looks like a wrench)
  - Add modifier -> Deform -> Displace
  - New
  - Srength 0.05
  - Midlevel 0.1
- Texture properties
  - Open and Choose the elevation .jpg
- Modifier
  - Add modifier -> Generate -> Subdivision surface
  - Right click on the object and Shade smooth

- Materials tab
  - New
  - In base color click the dot. Image texture. Open the second .jpg file you exported.

- Choose amonge the spheres above the nagivation tools, the Display render preview (the one on the right)


### Blender for Archaeology


#### Blender tutorials
- [Reconstructing archaeology Baalshamin temple (Palmyra) in Blender](https://www.youtube.com/watch?v=XfRsfwipq_0)
- [How to Create 3D Terrain with Google Maps and Blender!](https://www.youtube.com/watch?v=Mj7Z1P2hUWk&ab_channel=CGGeek)
- [Blender GIS - introduction and complete workflow](https://www.youtube.com/watch?v=u8Fg-u-VWUE)
- [QGIS User 0036 - QGIS and Blender](https://www.youtube.com/watch?v=AJJNX243k9E&ab_channel=KlasKarlsson)
- [Blender software: Pot reconstruction](https://youtu.be/eO90Qjfff2Y?t=1640) as part of the 3D Modelling of Synoikisis
- [Geometry Nodes Procedural Modelling [Ancient Greek Column]](https://www.youtube.com/watch?v=tA6NS3Y6jzA&ab_channel=KaizenTutorials)
- [Ancient Greek Column in Blender [3D Modeling]](https://www.youtube.com/watch?v=R9dKc9JEJi4&ab_channel=F%C3%A1bioCarvalho)
- [3D Model In Minutes Blender 2.9 Gothic Columns & Arches](https://www.youtube.com/watch?v=VTgELK7Hi7o&ab_channel=3DTudor)
- [How to Use Curves in Blender](https://www.youtube.com/watch?v=Ve9h7-E8EuM&ab_channel=RyanKingArt)
- [Create Mirrored Duplicates Objects](https://www.youtube.com/watch?v=qn3zRuCs4kA&ab_channel=BlenderRookie)
