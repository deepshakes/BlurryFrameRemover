# BlurryFrameRemover
This script, based on [Adrian Rosebrock's script](https://www.pyimagesearch.com/2015/09/07/blur-detection-with-opencv/), is designed to scan through a folder of images and move any blurry frames into a seperate folder.

## Dependencies

- cv2
- imutils

## Usage

Place all of the frames that you want to test in the 'Images' directory.

In your command line, from the the location of your BlurryFrameRemover directory, you can run the program like so:
`python3 blurryframeremover.py --image [path to image folder] --threshold [threshold value (default 10)]`
For example:
`python3 blurryframeremover.py --image ./images --threshold 20`

The lower your threshold value, the stricter the blur detection gets. For example, the default is 10 but a value of 100+ will likely end up flagging most of your images as blurry.
