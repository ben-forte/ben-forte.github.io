# Exploring 3D Gaussian Splatting
<!-- # MiniFigure-PopMart Gaussian Splat -->
3D Gaussian Splatting (3DGS)

## Description
Captured using a mobile phone (Samsung S23+) and processed with [Software Name]. 
This scene demonstrates the ability of Gaussian Splatting to capture intricate foliage and natural lighting.

## Goal
Goal of this experiment

### (how does it work)
overf view how does it work ? 

## technical breakdown
### Camera and capture information
This is image sensor info

### Software and hardware used
this is s/w and h/w

### Processing pipeline
this is processing pipeline

#### Data Preparation
<!-- https://medium.com/@heyulei/camera-alignment-and-gaussian-splatting-training-89858549784a -->

input: image frames, videos
output: 
1. given a video , convert to image frame using ffmpeg
2. `convert.py` 

```bash
$HOME$/gaussian-splatting/data/
.
├── distorted
│   ├── database.db
│   └── sparse
├── images
│   ├── i000016.jpg
│   ├── i000018.jpg
│   ├── i000019.jpg
│   ├── i000020.jpg
│   ├── i000021.jpg
│   ├── i000023.jpg
│   ├── i000024.jpg
│   ├── i000026.jpg
│   ├── i000027.jpg
│   ├── i000028.jpg
│   ├── i000029.jpg
│   ├── i000030.jpg
│   ├── i000031.jpg
│   ├── i000032.jpg
│   ├── i000033.jpg
│   ├── i000034.jpg
│   ├── i000035.jpg
│   ├── i000036.jpg
│   ├── i000037.jpg
│   └── i000038.jpg
├── input
│   ├── i000001.jpg
│   ├── i000002.jpg
│   ├── i000003.jpg
│   ├── i000004.jpg
│   ├── i000005.jpg
│   ├── i000006.jpg
│   ├── i000007.jpg
│   ├── i000008.jpg
│   ├── i000009.jpg
│   ├── i000010.jpg
│   ├── i000011.jpg
│   ├── i000012.jpg
│   ├── i000013.jpg
│   ├── i000014.jpg
│   ├── i000015.jpg
│   ├── i000016.jpg
│   ├── i000017.jpg
│   ├── i000018.jpg
│   ├── i000019.jpg
│   ├── i000020.jpg
│   ├── i000021.jpg
│   ├── i000022.jpg
│   ├── i000023.jpg
│   ├── i000024.jpg
│   ├── i000025.jpg
│   ├── i000026.jpg
│   ├── i000027.jpg
│   ├── i000028.jpg
│   ├── i000029.jpg
│   ├── i000030.jpg
│   ├── i000031.jpg
│   ├── i000032.jpg
│   ├── i000033.jpg
│   ├── i000034.jpg
│   ├── i000035.jpg
│   ├── i000036.jpg
│   ├── i000037.jpg
│   └── i000038.jpg
├── run-colmap-geometric.sh
├── run-colmap-photometric.sh
├── sparse
│   └── 0
└── stereo
    ├── consistency_graphs
    ├── depth_maps
    ├── fusion.cfg
    ├── normal_maps
    └── patch-match.cfg
```

### Information concerning optimization.


## Challenges and solutions
this is challenges

### Image capturing
golden reules of phogrammetry [ref](https://youtu.be/oqPzkoIOoZA?si=dFTg2FgGmJGF-6MT)

* 80% image overlap
* 30 deg max camera rotation
* good overlap = each point has to be visible on min. 3 images
* do not shoot panorama style (as phogrammetry is created based on parallax. panorame does not have offset)
* Raw image capture (more info than jpeg) despite more storage

Cyril 60/20 (side, between rows), 90/80 ?

Reference
[1] [Capture Images for Gaussian Splatting, Yulei He](https://medium.com/@heyulei/capture-images-for-gaussian-splatting-81d081bbc826)

https://codesandbox.io/p/github/mkkellogg/GaussianSplats3D/main