---
title: Download Instruction of ObjectFolder-Real
# subtitle: 
featured_image: 
---

### About ObjectFolder Real

### Dataset Download and Preparation

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



