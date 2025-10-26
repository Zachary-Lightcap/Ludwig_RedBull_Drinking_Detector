# Ludwig_RedBull_Drinking_Detector
Program and fine-tuned Convolutional Neural Network to detect when Ludwig drinks a Red Bull on stream.

## Currently
Bare-bones proof of concept where videos have to be manually uploaded, and clips have to be downloaded by hand.
Code currently runs in Google Colab to utilize GPUs for model training and CPU for the rest of the running.
Many clips generated -- a lot of false positives.
Most of the data comes from the YOLO model itself to detect a person, and a further fine-tuned YOLO model to detect the cans.

## How to Run
Download files and upload to Google Colab
Run important Cells for either further training, dataset tuning, or running the model.
If you want to use your own data pulls, insert your own API key.

## Future work 
- [ ] Gather Ludwig drinking Red Bull Dataset
- [ ] Label the data manually and create bounding boxes
- [ ] Improve object detection through background frame blurring and other methodologies
- [ ] Change from a 2-model solution to a singular YOLO model solution
- [ ] Simplify the process of uploading videos and gathering clips.
- [ ] Tune clip sizes.
