
Question-1 :

Cloud Computing for Deep Learning 
(a)	Elasticity and Scalability in Cloud Computing for Deep Learning 
•	Elasticity refers to the ability of a cloud computing system to automatically adjust resources (such as compute power, storage, and networking) based on demand. For deep learning, this means dynamically scaling up GPUs/TPUs during model training and scaling down when the demand decreases, optimizing cost efficiency.
•	Scalability is the capacity of a system to handle an increasing workload by adding more resources, either vertically (upgrading existing hardware) or horizontally (adding more machines). In deep learning, scalability ensures that models can be trained on massive datasets efficiently by distributing workloads across multiple cloud instances.



(b)	Comparison of AWS Sage Maker, Google Vertex AI, and Microsoft Azure Machine Learning Studio 

Feature	AWS Sage Maker	Google Vertex AI	Microsoft	Azure	ML Studio
Ease of Use	Provides pre-built Jupyter notebooks and automated ML capabilities.	Simplifies end-to-end AI workflows with AutoML and pipelines.	Offers a no-code UI along with support for advanced ML pipelines.
Compute Support	Supports CPU, GPU, and AWS Inferentia chips for cost-effective inference.	Offers TPUs, GPUs, and CPUs for AI model training and deployment.	Provides flexible compute options, including NVIDIA GPUs and FPGAs.
AutoML Capabilities	Includes built-in AutoML for training without deep expertise.	Strong AutoML support with hyperparameter tuning.	Advanced AutoML with drag-and-drop features.
Model Deployment	One-click deployment with endpoints for real- time inference.	Seamless model deployment via AI pipelines.	Supports real-time and batch inference with MLOps integration.
Integration & Ecosystem	Deep integration with AWS services (S3, Lambda, EC2, etc.).	Native support for Google Cloud services (BigQuery, Dataflow, etc.).	Well-integrated with Azure services (Power BI, Cognitive Services, etc.).
Pricing	Pay-as-you-go pricing with spot instance discounts.	Flexible pricing based on usage; discounts for sustained use.	Consumption-based pricing with enterprise discounts.
 
Each platform has strengths depending on specific needs:
•	AWS SageMaker: Best for users already in the AWS ecosystem. It provides end-to-end machine learning services, including built-in algorithms, automated model tuning, and easy AWS storage and compute integration.
•	Google Vertex AI: Optimized for large-scale AI workloads and deep learning applications, especially with TPUs (Tensor Processing Units). It offers seamless integration with Google Cloud services and a unified AI platform for model training, deployment, and monitoring.
•	Azure Machine Learning Studio: Well-suited for enterprises using Microsoft services. It provides robust MLOps capabilities, AutoML features, and strong integration with tools like Power BI and Azure DevOps.


Question -2 

Convolution Operations with Different Parameters:

Input Matrix: A 5×5 matrix is used as input.
Kernel: A 3×3 kernel is applied for convolution.
Operations: Convolution is performed with:

Stride = 1, Padding = 'VALID': No padding, smaller output.
Stride = 1, Padding = 'SAME': Padding added to maintain input size.
Stride = 2, Padding = 'VALID': No padding, output shrinks further.
Stride = 2, Padding = 'SAME': Padding added, output size adjusted.

Output Feature Maps:
Each case produces a unique output feature map based on stride and padding.

Key Takeaway:
Stride controls how the kernel moves, and padding determines if the input size is preserved.

Question -3
Task 1: Edge Detection Using Sobel Filter
Input: A grayscale image is loaded.

Sobel Filters:
Sobel-X detects vertical edges.
Sobel-Y detects horizontal edges.

Output: Three images are displayed:
Original grayscale image.
Sobel-X edge detection.
Sobel-Y edge detection.

Task 2: Max Pooling and Average Pooling
Input: A random 4×4 matrix.
Max Pooling: Selects the maximum value in each 2×2 window.
Average Pooling: Calculates the average value in each 2×2 window.
Output: The original matrix, max-pooled matrix, and average-pooled matrix are printed.

Key Takeaway:
Sobel filters are great for edge detection.
Pooling reduces dimensionality while preserving important features.

Question-4
Task 1: Implement AlexNet

Layers:

Conv2D layers with ReLU activation.
MaxPooling layers for downsampling.
Fully Connected (Dense) layers with Dropout for regularization.
Softmax output layer for classification.
Purpose: A deep CNN for image classification.

Task 2: Implement ResNet-like Model

Residual Block:
Two Conv2D layers with skip connections.
Solves vanishing gradients in deep networks.

ResNet Architecture:
Starts with a Conv2D layer.
Uses two residual blocks.
Ends with Flatten, Dense, and Softmax layers.

Key Takeaway:

AlexNet is a classic deep CNN.
ResNet introduces skip connections for better training of deep networks.
