# This is a repository for a Kaggle competition

This repository contains my code and for the Kaggle competition [`TensorFlow - Help Protect the Great Barrier Reef`](https://www.kaggle.com/c/tensorflow-great-barrier-reef/overview) 

# Disclaimer
Feel free to take a look in this repository, but if you want better quality code, please go to [Kaggle competition code](https://www.kaggle.com/c/tensorflow-great-barrier-reef/code).

# Data

To get data, please download them here : https://www.kaggle.com/c/tensorflow-great-barrier-reef/data 

Then put them in the folder data

## Data VOC Format:
The notebook `data_transformation.ipynb` will transform the data to the format used by YOLOX `VOC`. *(Not yet tested)*

Please see the notebook for more information.

# YOLOX

I'm using the repository [YOLOX](https://github.com/Megvii-BaseDetection/YOLOX.git) as a submodule, So please run the commands :
```bash
$ git submodule init
$ git submodule update
```
I have also updated the requirements, so please install the ones outside the `YOLOX` submodule by running the command :
``` bash
$ pip install -U pip
$ pip install -r requirements.txt
```
If you noticed, I have also added `yolox_nano.pth` in the branch, it is just to simplify our life *(not a good habit, but for 7 MB only its fine)*, you can find more in the [YOLOX](https://github.com/Megvii-BaseDetection/YOLOX.git) repository.

# Execution order :
- get `YOLOX` submodule	
- get data
- `data_transformation.ipynb`
- `training.ipynb`

