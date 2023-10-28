---
class: 12
day: Thursday, November 2
title: 'Blender'
tags: 
---

## Assignment due: 
- Create a 3D model of an interesting object in Agistoft Metashape and upload it on Sketchfab.

## Before Class 
- Download [Blender](https://www.blender.org/download/)

## Notes 

#### Blender shortcuts
- Shift + A: Add
- Tab: Swift between Object Mode and Edit Mode
- Shift + R: Repeat

#### Creating a 3D model of Crete

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
  - Add modifier -> Difform -> Displace
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
