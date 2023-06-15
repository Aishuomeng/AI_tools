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
