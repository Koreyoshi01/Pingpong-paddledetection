# 乒乓球检测项目

## 文件说明

由于数据集过大，以及 PaddleDetection 文件夹中也带有数据集，还有推理输出和所有模型参数都过大，所以都被忽略了。在 submission 文件夹中有一组模型参数。

## .gitignore 配置
```
dataset/
PaddleDetection/dataset/
work/img/
work/export_model/
work/model/
work/ppq
```
## 数据集说明

数据集可在飞桨 AI Studio 下载。下载后，需将数据整理为以下结构：

```
dataset
├── train
│ ├── JPEGImages # 训练集图片
│ │ ├── img_name.png
│ │ ├── ...
│ ├── Annotations # 训练集标注（XML格式）
│ │ ├── img_name.xml
│ │ ├── ...
│ ├── train_annotations_coco.json # COCO 格式标注（推理用）
│ ├── train_list.txt # 训练/评估标注文件
│ ├── labels.txt
│ ├── game_1
│ │ ├── frames
│ │ ├── annotations.json
│ │ ├── ...
│ ├── ...
├── val
│ ├── JPEGImages # 验证集图片
│ │ ├── img_name.png
│ │ ├── ...
│ ├── Annotations # 验证集标注（XML格式）
│ │ ├── img_name.xml
│ │ ├── ...
│ ├── val_annotations_coco.json # COCO 格式标注（推理用）
│ ├── val_list.txt # 训练/评估标注文件
│ ├── labels.txt
│ ├── game_1
│ │ ├── frames
│ │ ├── annotations.json
│ │ ├── ...
│ ├── ...
```
