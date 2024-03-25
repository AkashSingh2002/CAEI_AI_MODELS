### YOLOv8?
![image](https://github.com/Ro-han12/CAEI_AI_MODELS/assets/95674406/e9291e99-1d30-41e5-a4d8-54ae7f960add)

The field of computer vision advances with the release of YOLOv8, a model that defines a new state of the art for object detection, instance segmentation, and classification.

Along with improvements to the model architecture itself, YOLOv8 introduces developers to a new friendly interface via a PIP package for using the YOLO model.

Here we will dive into the significance of YOLOv8 in the computer vision world, compare it to similar models in terms of accuracy, and discuss the recent changes in the YOLOv8 GitHub repository. Let's begin!

### What is YOLOv8?
YOLOv8 is the newest state-of-the-art YOLO model that can be used for object detection, image classification, and instance segmentation tasks. YOLOv8 was developed by Ultralytics, who also created the influential and industry-defining YOLOv5 model. YOLOv8 includes numerous architectural and developer experience changes and improvements over YOLOv5.

YOLOv8 is under active development as of writing this post, as Ultralytics work on new features and respond to feedback from the community. Indeed, when Ultralytics releases a model, it enjoys long-term support: the organization works with the community to make the model the best it can be.

### How YOLO Grew Into YOLOv8
The YOLO (You Only Look Once) series of models has become famous in the computer vision world. YOLO's fame is attributable to its considerable accuracy while maintaining a small model size. YOLO models can be trained on a single GPU, which makes it accessible to a wide range of developers. Machine learning practitioners can deploy it for low cost on edge hardware or in the cloud.

YOLO has been nurtured by the computer vision community since its first launch in 2015 by Joseph Redmond. In the early days (versions 1-4), YOLO was maintained in C code in a custom deep learning framework written by Redmond called Darknet.

YOLOv8 author, Glenn Jocher at Ultralytics, shadowed the YOLOv3 repo in PyTorch (a deep learning framework from Facebook). As the training in the shadow repo got better, Ultralytics eventually launched its own model: YOLOv5.

YOLOv5 quickly became the world's SOTA repo given its flexible Pythonic structure. This structure allowed the community to invent new modeling improvements and quickly share them across repository with similar PyTorch methods.

Along with strong model fundamentals, the YOLOv5 maintainers have been committed to supporting a healthy software ecosystem around the model. They actively fix issues and push the capabilities of the repository as the community demands.

In the last two years, various models branched off of the YOLOv5 PyTorch repository, including Scaled-YOLOv4, YOLOR, and YOLOv7. Other models emerged around the world out of their own PyTorch based implementations, such as YOLOX and YOLOv6. Along the way, each YOLO model has brought new SOTA techniques that continue to push the model's accuracy and efficiency.

Over the last six months, Ultralytics worked on researching the newest SOTA version of YOLO, YOLOv8. YOLOv8 was launched on January 10th, 2023.

### Why Should I Use YOLOv8?
Here are a few main reasons why you should consider using YOLOv8 for your next computer vision project:

YOLOv8 has a high rate of accuracy measured by Microsoft COCO and Roboflow 100.
YOLOv8 comes with a lot of developer-convenience features, from an easy-to-use CLI to a well-structured Python package.
There is a large community around YOLO and a growing community around the YOLOv8 model, meaning there are many people in computer vision circles who may be able to assist you when you need guidance.
YOLOv8 achieves strong accuracy on COCO. For example, the YOLOv8m model -- the medium model -- achieves a 50.2% mAP when measured on COCO. When evaluated against Roboflow 100, a dataset that specifically evaluates model performance on various task-specific domains, YOLOv8 scored substantially better than YOLOv5. More information on this is provided in our performance analysis later in the article.

Furthermore, the developer-convenience features in YOLOv8 are significant. As opposed to other models where tasks are split across many different Python files that you can execute, YOLOv8 comes with a CLI that makes training a model more intuitive. This is in addition to a Python package that provides a more seamless coding experience than prior models.

The community around YOLO is notable when you are considering a model to use. Many computer vision experts know about YOLO and how it works, and there is plenty of guidance online about using YOLO in practice. Although YOLOv8 is new as of writing this piece, there are many guides online that can help.

### YOLOv8 Architecture: A Deep Dive
YOLOv8 does not yet have a published paper, so we lack direct insight into the direct research methodology and ablation studies done during its creation. With that said, we analyzed the repository and information available about the model to start documenting what's new in YOLOv8.

If you want to peer into the code yourself, check out the YOLOv8 repository and you view this code differential to see how some of the research was done.

Here we provide a quick summary of impactful modeling updates and then we will look at the model's evaluation, which speaks for itself.

The following image made by GitHub user RangeKing shows a detailed vizualisation of the network's architecture.
![image](https://github.com/Ro-han12/CAEI_AI_MODELS/assets/95674406/47673f31-91d3-4fb1-b701-17130e4dc724)



### REFERENCES:
1. 'https://blog.roboflow.com/whats-new-in-yolov8/'
2.
