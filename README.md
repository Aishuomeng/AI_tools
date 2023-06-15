# AI_tools
A collection of small tools for image processing.
## 图像处理和标注程序

这段代码是一个用于处理图像和标注的简单图形界面程序。它提供了一个用户友好的界面，让用户能够方便地处理图像和标注数据。

### 功能说明

1. **图像预处理**：代码中的`preprocess_image`函数用于将图像调整为指定的目标分辨率，并进行填充，以适应不同尺寸的标注。
2. **标注点处理**：`preprocess_points`函数将标注点的坐标进行缩放和偏移，以适应预处理后的图像。
3. **绘制标注**：`draw_annotations`函数遍历图像文件夹中的每个图像，并根据相应的标注文件，在预处理后的图像上绘制标注。
4. **保存结果**：标注绘制完成后，将结果保存为带有透明度通道的 PNG 图像和对应的标签文件，方便后续使用和分析。

### 使用说明

1. **选择图像路径**：通过点击"选择文件夹"按钮，选择包含图像文件的文件夹。
2. **选择标注文件路径**：通过点击"选择文件夹"按钮，选择包含标注文件的文件夹。
3. **选择存储位置**：通过点击"选择文件夹"按钮，选择用于保存处理结果的文件夹。
4. **选择目标分辨率**：通过单选按钮选择目标分辨率选项，可以是"512x512"或"512x768"。
5. **开始处理**：点击"开始处理"按钮，程序将开始处理图像和标注数据，将结果保存在指定的存储位置中。

### 依赖库和模块

- numpy
- cv2 (OpenCV)
- os
- json
- tkinter
- tkinter.filedialog

### 代码结构

```python
# 导入所需的库和模块
# ...

# 定义辅助函数
# ...

# 定义主要的处理函数
# ...

# 定义处理的入口函数
# ...

# 创建图形界面窗口
# ...

# 运行图形界面主循环
# ...
# AI_tools
A collection of small tools for image processing.

## Image Processing and Annotation Program

This code is a simple graphical user interface program for image processing and annotation. It provides a user-friendly interface that allows users to conveniently manipulate images and annotation data.

### Functionality

1. **Image Preprocessing**: The `preprocess_image` function in the code is used to resize the image to the specified target resolution and perform padding to accommodate annotations of different sizes.
2. **Annotation Point Processing**: The `preprocess_points` function scales and offsets the coordinates of the annotation points to fit the preprocessed image.
3. **Drawing Annotations**: The `draw_annotations` function iterates through each image in the image folder and draws the annotations on the preprocessed image based on the corresponding annotation files.
4. **Saving Results**: After the annotations are drawn, the results are saved as PNG images with transparency channels and corresponding label files for future use and analysis.

### Usage Instructions

1. **Select Image Folder**: Click the "Select Folder" button to choose the folder containing the image files.
2. **Select Annotation Folder**: Click the "Select Folder" button to choose the folder containing the annotation files.
3. **Select Storage Location**: Click the "Select Folder" button to choose the folder where the processed results will be saved.
4. **Select Target Resolution**: Select the target resolution option using the radio buttons, either "512x512" or "512x768".
5. **Start Processing**: Click the "Start Processing" button to initiate the image and annotation data processing, and save the results in the specified storage location.

### Dependencies and Modules

- numpy
- cv2 (OpenCV)
- os
- json
- tkinter
- tkinter.filedialog

### Code Structure

```python
# Import required libraries and modules
# ...

# Define helper functions
# ...

# Define main processing functions
# ...

# Define the entry point for processing
# ...

# Create the graphical user interface window
# ...

# Run the main loop of the graphical user interface
# ...
