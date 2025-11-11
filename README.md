# Ludwig_RedBull_Drinking_Detector
Fine-tuned a Convolutional Neural Network to detect when Ludwig drinks a Red Bull on stream and automatically save the clips.

## Currently
Early model version fine-tuned on a small labeled dataset where videos have to be manually uploaded, and clips have to be downloaded by hand.
Training of the model was run in Google Colab to utilize GPUs; the rest of the notebook has been updated to run on a local machine.
Some results are included, as well as an example of some clips pulled from a single full video uploaded. Ne
Most of the data comes from the YOLO (You Only Look Once) model itself to detect a person, which adds in synthetic Red Bull can data to fine-tune the model.

## How to Run
Download the notebook and best_weights.pt and run it on either Google Colab or a local machine. If running on a local machine, note that dependencies must be downloaded.
Run important Cells for either further training, dataset tuning, or running the model. However, a dataset would need to be manually provided to further tune.

## Future work 
- [x] Gather Ludwig drinking Red Bull Dataset
- [x] Label the data manually and create bounding boxes
- [ ] Improve object detection through background frame blurring and other methodologies
- [x] Change from a 2-model solution to a singular YOLO model solution
- [ ] Simplify the process of uploading videos and gathering clips (potentially creating a website).
- [ ] Tune clip sizes.
