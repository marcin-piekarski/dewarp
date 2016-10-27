# dewarp 360

## what is this?
dewarping & stitching fisheye images

## methodology

* 1) split dual fish eyes into two images
* 2) dewarp each image
* 3) align & stitch each image

## run

first, dewarp images. the following command will create two dewarped images - DeWarp0.png and DeWarp1.png - in the "output" folder.
```
python defish.py images/360_0289.png
```

then, stitch images. the following command will create a stitched image in "final" folder. for more information, go https://github.com/marcpare/stitch

```
python stitch.py output/DeWarp0.png output/DeWarp0.png
```