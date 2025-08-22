# 🚦 Traffic Sign Image Classification (97% Accuracy with CNN)

This project implements a **Convolutional Neural Network (CNN)** to classify German traffic sign images from the [GTSRB dataset](https://benchmark.ini.rub.de/gtsrb_news.html). The trained model achieves **97%+ accuracy** on the test set, making it suitable for real-world traffic sign recognition tasks such as **autonomous driving** and **driver assistance systems**.

---

## 📂 Project Structure

1. **Download and Imports**  
   Import all necessary libraries (TensorFlow, Keras, OpenCV, NumPy, Pandas, etc.).

2. **Functions**  
   - Utility function for timestamps.  
   - `plot_performance()` function to visualize training and validation accuracy/loss.

3. **Loading Dataset**  
   - Load and preprocess the **German Traffic Sign Recognition Benchmark (GTSRB)** dataset.  
   - Resize images to **30x30 pixels**.  
   - Store images (`data`) and labels (`labels`).

4. **Data Splitting & Conversion**  
   - Split data into **training** and **testing** sets.  
   - One-hot encode labels for classification.

5. **Model Creation & Compilation**  
   - A CNN architecture with:  
     - Multiple **Conv2D** layers  
     - **MaxPooling** layers  
     - **Dropout** layers to reduce overfitting  
     - Fully connected **Dense** layers  
   - Compiled with `categorical_crossentropy` loss and `Adam` optimizer.

6. **Training the Model**  
   - Trained for **35 epochs** with batch size **128** on GPU.  
   - Achieved **99% validation accuracy** during training.

7. **Performance Visualization**  
   - Training and validation **accuracy/loss curves** plotted using Matplotlib.

8. **Evaluation on Test Dataset**  
   - Tested on official GTSRB test set.  
   - Achieved **97.28% test accuracy**.

9. **Saving the Model**  
   - Final trained model is saved as `traffic_classifier.h5`.

---

## 📊 Results

- **Validation Accuracy:** ~99%  
- **Test Accuracy:** ~97.28%  
- Robust against multiple traffic sign classes (**43 categories**).


ects
