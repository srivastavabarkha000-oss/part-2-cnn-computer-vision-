# Part 2: Computer Vision Problem Formulation and CNN Prototype
**Task 6: CNN Concept Explanation**

Q. What is convolution?
Convolution is the process where a CNN scans an image using small filters (also called kernels) to detect important visual features.

These filters help identify patterns such as:
- edges
- lines
- textures
- scratches
- dents
- shapes

Instead of looking at the whole image at once, the CNN learns small visual patterns step by step.

Example convolution filter: 3×3
A filter moves across the image pixel by pixel and produces a feature map showing where important patterns are found. 
The filter is a 3x3 matrix which performs mathematical operations to detect features.

Q. Why is pooling used?
Pooling is used to reduce the size of feature maps while keeping the most important information.

The most common type is Max Pooling.

Example pooling size: 2×2
Benefits of pooling:

- reduces computation
- speeds up training
- reduces overfitting
- keeps important features

Pooling helps the CNN focus on dominant visual patterns instead of unnecessary details. 

Q. Why is ReLU commonly used in CNNs?
ReLU (Rectified Linear Unit) is an activation function that introduces non-linearity into the network.

ReLU function: f(x)=max(0,x)

This means:
- negative values become 0
- positive values remain unchanged

Why ReLU is popular:
- It is simple and fast
- It helps deep networks learn complex patterns
- It reduces the vanishing gradient problem
- It improves training efficiency

Without ReLU, the CNN would behave like a simple linear model and would not learn complex image features effectively.
While tanh keeps:
- negative values negative
- positive values positive
And sigmoid function has a strong vanishing gradient.

Q. Why are CNNs better than regular feed-forward networks for image data?
CNNs are better for image data because they are specifically designed to process **spatial visual** information.

Advantages of CNNs
**1. Automatic Feature Extraction**
CNNs automatically learn important image features such as:
- edges
- textures
- defects
- shapes

Regular feed-forward networks cannot efficiently capture spatial image patterns.

**2. Fewer Parameters**
CNNs use shared filters, which greatly reduce the number of parameters compared to fully connected networks.

This makes CNNs:
- faster
- more memory efficient
- easier to train on images

**3. Spatial Understanding**
CNNs preserve relationships between nearby pixels.
This is important because image patterns depend on spatial structure.

Example:
- scratches appear as lines
- dents appear as circular depressions
- stains appear as irregular patches
CNNs can learn these visual structures effectively.

**4. Better Performance on Images**

CNNs usually achieve much higher accuracy than regular neural networks on image classification tasks because they are specialized for visual learning.

**Final Summary**
CNNs are powerful deep learning models for computer vision because they:
- extract visual features using convolution
- reduce dimensions using pooling
- learn complex patterns using ReLU
- efficiently process image structure better than traditional feed-forward networks

This makes CNNs highly suitable for manufacturing defect detection and image classification tasks.

**Task 7: Business Use Case Mapping**

