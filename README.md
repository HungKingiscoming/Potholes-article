# A comparison of semantics segmentation approaches for pothole detection.
### Potholes Problems Overview
<div align="justify">
A pothole is a depression or cavity in the road surface that gradually develops as a result of water infiltration, repeated traffic load, and adverse weather conditions, leading to deterioration of the pavement. Potholes pose a significant threat to road safety, as they can damage vehicles, compromise driving comfort, and increase the risk of accidents by causing abrupt maneuvers or endangering cyclists and pedestrians.  
</div>


    
<!-- ![image](resources/pot.jpg) -->
<div align="center">
  <img src="./Resources/pot1.jpg" alt="Image 1" height="200" style="margin-right: 10px;">
  <img src="./Resources/pot2.jpg" alt="Image 2" height="200" style="margin: 0 10px;">
  <img src="./Resources/pot3.jpg" alt="Image 3" height="200" style="margin-left: 10px;">
</div>

<p align="center">
  Some samples about potholes.
</p>
<div align="justify">
So we provides a thorough comparison of various semantic segmentation techniques applied to pothole detection on road surfaces. The models evaluated encompass traditional CNN-based architectures, including U-Net, FPN, and DeepLabv3, as well as advanced Transformer-based approaches such as SegFormer, Swin-Unet, and Mask2Former.  
</div>

  
You can see the full version of reference through [paper](https://easychair.org/conferences2/submission_download?a=34672663&submission=7282567&upload=151756).  
### How semantics segmentation deals with those problems
<div align="justify">
  Timely identification and repair of potholes are crucial for preserving road infrastructure, maintaining smooth traffic flow, and minimizing vehicle damage.
</div>
<div align="justify">
  Recent advancements in deep learning have brought semantic segmentation to the forefront of computer vision, with widespread applications in detecting everyday objects such as vehicles and animals.
</div>
<div align="justify">
  While deep learning-based semantic segmentation has shown remarkable progress in various road imagery tasks (Patel, Dabhi & Adhvaryu, 2024), its targeted application for pothole detection remains relatively limited and underexplored.  
</div>
<div align="justify">
  In our experiments, all evaluated methods were trained and tested on two distinct datasets: the Potholes-Detection Dataset (PotholesDetection, 2024), which includes over 1,000 images of potholes, and the Pothole Mix Dataset (Ranieri, Moscoso Thompson & Biasotti, 2022), containing more than 4,000 images with varying resolutions. 
</div>
<div align="justify">
  Two datasets are published, you can download through 
  <a href="https://universe.roboflow.com/potholesdetection-aq76f/potholes-detection-ohg1g">Potholes-Detection</a> (Roboflow) and 
  <a href="https://data.mendeley.com/datasets/kfth5g2xk3/2">Pothole Mix Dataset</a> (Ranieri, Moscoso Thompson & Biasotti, 2022).
</div>
 

### Experimental Results  
<div align="justify">
  Deep Learning-Based Semantic Segmentation models can be classified into two main types: CNN-based methods (Unet, FPN, PSPNet, DeeplabV3 and DeeplabV3+) and Transformer-based models (Segformer, Mask2Former, Upernet and SwinUnet)   
</div>  

  
To obtain the results of all models on both datasets, we utilized Kaggle as the computing platform.  


Notebooks use Pothole-Detection dataset (Those notebook may not have equal results compared to our reference because of different runs) :

Unet: [Notebook](https://www.kaggle.com/code/giangtunhng/unet-potholes-detection)  

FPN: [Notebook](https://www.kaggle.com/code/giangtunhng/fpn-potholes-detetion)  

PSPNet: [Notebook](https://www.kaggle.com/code/giangtunhng/unet-potholes-detection)  

DeepLabV3+:[Notebook](https://www.kaggle.com/code/giangtunhng/deeplabv3-potholesdetection)  

DeepLabV3: [Notebook](https://www.kaggle.com/code/giangtunhng/deeplabv3-potholes-detection)  

Segformer: [Notebook](https://www.kaggle.com/code/giangtunhng/segformer-potholes-detection)  
 
You can see our detection score of compared semantic segmentation models on the Potholes-Detection dataset:
| Method       | Accuracy (%) | mIoU (%) | Dice (%) |
|--------------|--------------|----------|-----------|
| Unet         | 87.46        | 82.00    | 89.54     |
| FPN          | 87.76        | 81.90    | 89.47     |
| PSPNet       | 85.45        | 79.90    | 88.08     |
| DeepLabV3+   | 87.28        | 81.79    | 89.40     |
| DeepLabV3    | 86.98        | 81.70    | 89.34     |
| SegFormer    | 87.52        | 82.45    | 89.85     |
| Mask2Former  | 88.33        | 83.06    | 90.26     |
| Upernet      | 88.00        | 86.73    | 85.60     |
| SwinUnet     | 86.44        | 87.15    | 96.89     |


Notebooks use Pothole Mix Dataset (Those notebook may not have equal results compared to our reference because of different runs) :


Unet: [Notebook](https://www.kaggle.com/code/giangtunhng/unet-potholes-detection)  

FPN: [Notebook](https://www.kaggle.com/code/giangtunhng/fpn-potholes-detetion)  

PSPNet: [Notebook](https://www.kaggle.com/code/giangtunhng/unet-potholes-detection)  

DeepLabV3+:[Notebook](https://www.kaggle.com/code/giangtunhng/deeplabv3-potholesdetection)  

DeepLabV3: [Notebook](https://www.kaggle.com/code/giangtunhng/deeplabv3-potholes-detection)  

Segformer: [Notebook](https://www.kaggle.com/code/giangtunhng/segformer-potholes-detection)

You can see our detection score of compared semantic segmentation models on the Pothole Mix Dataset:
| Method       | Accuracy (%) | mIoU (%) | Dice (%) |
|--------------|--------------|----------|-----------|
| Unet         | 82.35        | 78.46    | 86.43     |
| FPN          | 82.17        | 77.81    | 85.92     |
| PSPNet       | 78.43        | 74.10    | 82.78     |
| DeepLabV3+   | 82.84        | 74.87    | 83.50     |
| DeepLabV3    | 82.84        | 84.87    | 83.50     |
| SegFormer    | 84.11        | 76.54    | 84.90     |
| Mask2Former  | 83.40        | 77.52    | 85.69     |
| Upernet      | 75.94        | 72.51    | 77.94     |
| SwinUnet     | 97.41        | 97.19    | 98.57     |

<!-- ![image](resources/pot.jpg) -->
<div align="center">
  <img src="./Resources/pot4.jfif" alt="Image 1" height="500" weight="600" style="margin-right: 10px;">
</div>

<p align="center">
  Visualize some results
</p>

### Conclusion
<div align="justify">
  Despite the promising performance of the models, challenges such as detecting small and blurry potholes persist,
underscoring the need for further research. Enhancing model capabilities to address these limitations is expected to improve
pothole detection performance across diverse and complex real-world environments
</div>
