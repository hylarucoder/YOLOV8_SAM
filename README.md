# YOLOV8_SAM
yolov8 model with SAM meta


Use yolov8 & SAM model to get segmention for custom model


# installation

```
pip install ultrlytics
pip install 'git+https://github.com/facebookresearch/segment-anything.git'

```

## Download weights 
```
 !wget -P images https://raw.githubusercontent.com/facebookresearch/segment-anything/main/notebooks/images/truck.jpg
 !wget -P images https://raw.githubusercontent.com/facebookresearch/segment-anything/main/notebooks/images/groceries.jpg       
 !wget https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth
```

## Test on Image

```
python main.py
```


## Results
<img width="312" alt="image" src="https://user-images.githubusercontent.com/62583018/232183468-d1abeb02-43d0-471a-9fce-e0e40eac69a5.png">

Bounding box: [478, 1280, 182, 76]
Segmentation mask: [631, 1280, 630, 1281, 629, 1281, 628, 1282, 626, 1282, 625, 1283, 622, 1283, 621, 1284, 619, 1284, 618, 1285, 615, 1285, 614, 1286, 612, 1286, 611, 1287, 609, 1287, 608, 1288, 607, 1288, 606, 1289, 604, 1289, 603, 1290, 602, 1290, 601, 1291, 599, 1291, 598, 1292, 596, 1292, 595, 1293, 593, 1293, 592, 1294, 590, 1294, 589, 1295, 587, 1295, 586, 1296, 584, 1296, 583, 1297, 579, 1297, 578, 1298, 576, 1298, 575, 1299, 574, 1299, 573, 1300, 571, 1300, 570, 1301, 569, 1301, 568, 1302, 566, 1302, 565, 1303, 563, 1303, 562, 1304, 561, 1304, 560, 1305, 558, 1305, 557, 1306, 555, 1306, 554, 1307, 552, 1307, 551, 1308, 548, 1308, 547, 1309, 544, 1309, 543, 1310, 541, 1310, 540, 1311, 538, 1311, 537, 1312, 535, 1312, 534, 1313, 533, 1313, 532, 1314, 530, 1314, 529, 1315, 526, 1315, 525, 1316, 524, 1316, 523, 1317, 522, 1317, 521, 1318, 520, 1318, 519, 1319, 518, 1319, 516, 1321, 515, 1321, 514, 1322, 512, 1322, 511, 1323, 510, 1323, 509, 1324, 507, 1324, 506, 1325, 504, 1325, 503, 1326, 502, 1326, 501, 1327, 497, 1327, 496, 1328, 492, 1328, 491, 1329, 490, 1329, 489, 1330, 484, 1330, 483, 1331, 482, 1331, 479, 1334, 479, 1335, 478, 1336, 478, 1346, 479, 1347, 479, 1349, 480, 1350, 480, 1352, 482, 1354, 486, 1354, 487, 1355, 492, 1355, 493, 1354, 496, 1354, 497, 1353, 499, 1353, 501, 1351, 506, 1351, 507, 1352, 510, 1352, 511, 1351, 514, 1351, 515, 1350, 517, 1350, 518, 1349, 519, 1349, 520, 1348, 521, 1348, 522, 1347, 523, 1347, 524, 1346, 526, 1346, 527, 1345, 528, 1345, 529, 1344, 532, 1344, 533, 1343, 536, 1343, 537, 1342, 539, 1342, 540, 1341, 542, 1341, 543, 1340, 545, 1340, 546, 1339, 548, 1339, 549, 1338, 550, 1338, 551, 1337, 553, 1337, 554, 1336, 556, 1336, 557, 1335, 558, 1335, 559, 1334, 561, 1334, 562, 1333, 564, 1333, 565, 1332, 567, 1332, 568, 1331, 570, 1331, 571, 1330, 573, 1330, 574, 1329, 575, 1329, 576, 1328, 579, 1328, 580, 1327, 582, 1327, 583, 1326, 584, 1326, 585, 1325, 587, 1325, 588, 1324, 589, 1324, 590, 1323, 591, 1323, 592, 1322, 595, 1322, 596, 1321, 598, 1321, 599, 1320, 601, 1320, 602, 1319, 605, 1319, 606, 1318, 609, 1318, 610, 1317, 612, 1317, 613, 1316, 616, 1316, 617, 1315, 618, 1315, 619, 1314, 621, 1314, 622, 1313, 623, 1313, 625, 1311, 626, 1311, 627, 1310, 628, 1310, 629, 1309, 631, 1309, 632, 1308, 634, 1308, 635, 1307, 638, 1307, 639, 1306, 641, 1306, 642, 1305, 644, 1305, 645, 1304, 646, 1304, 647, 1303, 648, 1303, 650, 1301, 651, 1301, 652, 1300, 653, 1300, 654, 1299, 655, 1299, 658, 1296, 658, 1293, 659, 1292, 659, 1290, 656, 1287, 655, 1287, 654, 1286, 653, 1286, 652, 1285, 651, 1285, 650, 1284, 649, 1284, 648, 1283, 646, 1283, 645, 1282, 644, 1282, 643, 1281, 641, 1281, 640, 1280]

### TODO


```
- Doing annotations on multiple images  - Done
- Add support for saving annotations in yolo format
- Support jsno format for segmentation model trainig

```

### refrence
```
https://github.com/facebookresearch/segment-anything
https://github.com/ultralytics/ultralytics
````
