state management: 

texture, material shader

alpha blending 
culling

texture atlas


Plane ? 

Plane and sphere intersection 

Plane and 3d point relationship ? 

on plane ? pos/neg side



BoundingVolumes

aabb

bounding sphere 

Fustrum: 
6 planes

how to create 6 planes from the group of parameters

Point with Fustrum ? if one of them is in the negative space false

Bounding sphere with Fustrum, center + radius

Bounding box with Fustrum ? 8 points test


SceneGraph : data structure

Binary space partition tree ? 
creating bsp tree is like Binary Search Tree 

Input is list of polygons like array of numbers in bst

How to choose the splitting plane is critical > 

balanced tree 

every polygon 




QuadTree 

create QuadTree from array of polygons'
each node carrys: aabb 

issue is polygon span multiple nodes: split polygons into two sets



How to cull quadTree with fustrum

fustrum intersection with aabb . 

only the leaf node carrys real polygon list


Terrain use case




Octree vs QuadTree ? 

Octree is for scene having polygons above the fustrum '''


Texture compression

LOD

Occulusion culling

strike a balance each pair needs to do occulusion 
