# My-Models
### 1. **DenseNet**
- Implementation of DenseNet, which utilizes dense connections to improve gradient flow and reduce the number of parameters.
- Variants available:
  - `DenseNet121`
  - `DenseNet169`
  - `DenseNet201`
  - `DenseNet161`
  - `DenseNet (CIFAR-10 specific)`

### 2. **GoogLeNet**
- Implementation of GoogLeNet, featuring the Inception module for efficient multi-scale feature extraction.

## **Training the Models**

### **Requirements**
- Python 3.8+
- PyTorch 1.12+
- torchvision
- CUDA (optional for GPU acceleration)

## **Features**

1. **Data Augmentation**:
   - Random cropping and horizontal flipping for CIFAR-10 training data.
2. **Learning Rate Scheduler**:
   - Cosine annealing to dynamically adjust the learning rate.
3. **Checkpointing**:
   - Automatically saves the best model based on test accuracy.
4. **Multi-GPU Support**:
   - Uses `torch.nn.DataParallel` for leveraging multiple GPUs.

---

## **Results**

### DenseNet (CIFAR-10)
- Achieves state-of-the-art accuracy with reduced computational cost due to dense connections.

### GoogLeNet (CIFAR-10)
- Efficient multi-scale feature extraction results in competitive accuracy.

