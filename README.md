# COVID-19 Face Mask Detector

![samples](images/testmask.gif)
## Prerequisites 

* `Python` version 2.7 or 3.5
* `Torch` version 1.0
* `Pytorch-lighting` version 0.9
 
 #### Installing Prerequisites 

`pip install -r requirements.txt`

# Reproduction
```Shell
git clone https://github.com/animesh-007/mask_detection.git
cd covid-mask-detector

# Download dataset and export it to pandas DataFrame
python -m covid-mask-detector.data_preparation
```
## Training

```Shell
python -m covid-mask-detector.train
```

## Testing on videos
```sh
python -m covid-mask-detector.video modelPath videoPath
```

### Usage
```
Usage: video.py [OPTIONS] MODELPATH VIDEOPATH

  modelPath: path to model.ckpt

  videoPath: path to video file to annotate

Options:
  --output PATH  specify output path to save video with annotations
```


