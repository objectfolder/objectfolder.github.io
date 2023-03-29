---
title: ObjectFolder-Real Download Instruction
# subtitle: 
featured_image: /assets/img/objectfolder/ObjectFolder-Real.jpg
---

### About ObjectFolder-Real
The ObjectFolder Real dataset contains multisensory data collected from 100 real-world household objects. The visual data for each object include three high-quality 3D meshes of different resolutions and an HD video recording of the object rotating in a lightbox; The acoustic data for each object include impact sound recordings recorded at 30–50 points of the object, each of which is 6s long and is accompanied by the coordinate of the striking location on the object mesh, ground-truth contact force profile, and the accompanying video for the impact. The tactile data for each object include tactile readings at the same 30–50 points of the object, with each tactile reading as a video of the tactile RGB images that record the entire gel deformation process and is accompanied by two videos of the contact process from an in-hand camera and a third-view camera.

### Dataset Download and Preparation

Use the following command to download the 3D meshes of the 100 objects (you may choose original or simplified versions):

```sh
# ~16K faces per mesh
wget https://download.cs.stanford.edu/viscam/ObjectFolder_Real/mesh/mesh_16k.tar.gz
tar -xvf mesh_16k.tar.gz
# ~64K faces per mesh
wget https://download.cs.stanford.edu/viscam/ObjectFolder_Real/mesh/mesh_64k.tar.gz
tar -xvf mesh_64k.tar.gz
# Full
wget https://download.cs.stanford.edu/viscam/ObjectFolder_Real/mesh/mesh_full.tar.gz
tar -xvf mesh_full.tar.gz
```

Use the following command to download the visual videos of the 100 objects:

```sh
wget https://download.cs.stanford.edu/viscam/ObjectFolder_Real/vision/videos_1_100.tar.gz
tar -xvf videos_1_100.tar.gz
```

Use the following command to download the acoustic data of the first 10 objects:

```sh
wget https://download.cs.stanford.edu/viscam/ObjectFolder_Real/audio/audio_data_1_10.tar.gz
tar -xvf audio_data_1_10.tar.gz
```

Use the following command to download the tactile data of the first 10 objects:

```sh
wget https://download.cs.stanford.edu/viscam/ObjectFolder_Real/tactile/tactile_data_1_10.tar.gz
tar -xvf tactile_data_1_10.tar.gz
```

Similarly, use the following command to download acoustic/tactile data from 11-100:

```sh
# replace X with a value in [10,20,30,40,50,60,70,80,90]
wget https://download.cs.stanford.edu/viscam/ObjectFolder_Real/audio/audio_data_[X+1]_[X+10].tar.gz
tar -xvf audio_data_[X+1]_[X+10].tar.gz
wget https://download.cs.stanford.edu/viscam/ObjectFolder_Real/tactile/tactile_data_[X+1]_[X+10].tar.gz
tar -xvf tactile_data_[X+1]_[X+10].tar.gz
```

### Full List of ObjectFolder Real

| Index |          Name          |   Material    | Index |        Name        |   Material    | Index |        Name         |   Material    |
| :---: | :--------------------: | :-----------: | :---: | :----------------: | :-----------: | :---: | :-----------------: | :-----------: |
|   1   |       Soup_Spoon       |    Ceramic    |  41   |    Wrench_Large    |     Steel     |  81   |  Utensil_Container  |     Wood      |
|   2   |          Bowl          |    Ceramic    |  42   |       Pestle       |     Iron      |  82   |         Can         |     Glass     |
|   3   |      Salad_Plate       |    Ceramic    |  43   |       Mortar       |     Iron      |  83   |    Potato_Masher    |     Steel     |
|   4   |      Dinner_Plate      |    Ceramic    |  44   |     Sculpture      |     Iron      |  84   |       Skimmer       |     Steel     |
|   5   |       Hair_Comb        |     Wood      |  45   |       Ladle        |     Iron      |  85   |    Pasta_Server     |     Steel     |
|   6   |       Blue_Bowl        |     Glass     |  46   |      Spatula       |     Iron      |  86   |    Slotted_Spoon    |     Steel     |
|   7   |    Decorative_Plate    |     Glass     |  47   |  Decorative_Cast   |     Iron      |  87   |    Solid_Turner     |     Steel     |
|   8   |      Mixing_Bowl       |    Ceramic    |  48   | Mixing_Bowl_Large  |    Plastic    |  88   |        Ladle        |     Steel     |
|   9   |      Serving_Bowl      |    Ceramic    |  49   | Mixing_Bowl_Middle |    Plastic    |  89   |     Solid_Spoon     |     Steel     |
|  10   |       Soup_Bowl        |    Ceramic    |  50   | Mixing_Bowl_Small  |    Plastic    |  90   |   Slotted_Turner    |     Steel     |
|  11   |     Strainer_Spoon     |     Wood      |  51   |     Fruit_Bowl     |     Glass     |  91   |     Glass_Green     |     Glass     |
|  12   |       Soup_Ladle       |     Wood      |  52   |     Fork_Small     |     Steel     |  92   |      Glass_Red      |     Glass     |
|  13   |     Serving_Spoon      |     Wood      |  53   |     Fork_Large     |     Steel     |  93   |        Vase         |     Glass     |
|  14   |       Salad_Fork       |     Wood      |  54   |    Spoon_Small     |     Steel     |  94   |     Salad_Bowl      |     Glass     |
|  15   |      Mixing_Spoon      |     Wood      |  55   |    Spoon_Large     |     Steel     |  95   |        Scoop        | Polycarbonate |
|  16   |     Frying_Spatula     |     Wood      |  56   |    Knife_Large     |    Plastic    |  96   |       Box_Lid       | Polycarbonate |
|  17   |     8Inch_Skillet      |     Iron      |  57   |    Knife_Middle    |    Plastic    |  97   |  Stanford_Frisbee   |    Plastic    |
|  18   | 10_dot_25Inch_Skillet  |     Iron      |  58   |    Knife_Small     |    Plastic    |  98   |     Kettlebell      |     Iron      |
|  19   |  10_dot_5Inch_Griddle  |     Iron      |  59   |     Soap_Dish      |     Glass     |  99   |  Trim_Removal_Tool  |    Plastic    |
|  20   |       Dutch_Oven       |     Iron      |  60   |     Beer_Glass     |     Glass     |  100  | Trim_Removal_Tool_2 |    Plastic    |
|  21   |     Dutch_Oven_Lid     |     Iron      |  61   |  Container_Large   |    Ceramic    |       |                     |               |
|  22   |      Rinsing_Cup       |     Glass     |  62   |  Container_Middle  |    Ceramic    |       |                     |               |
|  23   |       Hand_Scoop       |    Plastic    |  63   |  Container_Small   |    Ceramic    |       |                     |               |
|  24   |  Shovel_Toy_Red_Large  |    Plastic    |  64   |        Mug         |    Ceramic    |       |                     |               |
|  25   | Shovel_Toy_Green_Small |    Plastic    |  65   |        Vase        |    Ceramic    |       |                     |               |
|  26   |      Handle_Spoon      | Polycarbonate |  66   |    Plate_Handle    |     Iron      |       |                     |               |
|  27   |      Round_Plate       |     Wood      |  67   |       Plate        |     Iron      |       |                     |               |
|  28   |      Square_Plate      |     Wood      |  68   |     Plate_Base     |     Wood      |       |                     |               |
|  29   |  Cutting_Board_Large   |     Wood      |  69   |   Display_Stand    |     Iron      |       |                     |               |
|  30   |  Cutting_Board_Middle  |     Wood      |  70   |    Drop_Funnel     | Polycarbonate |       |                     |               |
|  31   |  Cutting_Board_Small   |     Wood      |  71   |   Container_Lid    | Polycarbonate |       |                     |               |
|  32   |       Wine_Glass       |     Wood      |  72   |      Food_Pan      | Polycarbonate |       |                     |               |
|  33   |      Drinking_Cup      |     Wood      |  73   |  Flowerpot_Large   |    Ceramic    |       |                     |               |
|  34   |        Beer_Mug        |     Wood      |  74   |  Flowerpot_Small   |    Ceramic    |       |                     |               |
|  35   |   Portion_Cup_Brown    | Polycarbonate |  75   |     Vase_Green     |    Ceramic    |       |                     |               |
|  36   |   Portion_Cup_White    | Polycarbonate |  76   |     Vase_Blue      |    Ceramic    |       |                     |               |
|  37   |        Cake_Pan        |     Steel     |  77   |    Vase_Orange     |    Ceramic    |       |                     |               |
|  38   |        Loaf_Pan        |     Steel     |  78   |     Swan_Large     |    Ceramic    |       |                     |               |
|  39   |      Wrench_Small      |     Steel     |  79   |     Swan_Small     |    Ceramic    |       |                     |               |
|  40   |     Wrench_Middle      |     Steel     |  80   |    Spoon_Holder    |     Wood      |       |                     |               |
