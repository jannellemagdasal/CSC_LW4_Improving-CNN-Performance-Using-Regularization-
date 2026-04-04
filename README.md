# CSC_LW4 — Improving CNN Performance Using Regularization

## Activity 1: Evaluation Metrics + Visualization

---

### Part 1: Load Your Saved Model

Mounted Google Drive and loaded the model.

![Part 1](https://github.com/user-attachments/assets/9e481cff-d443-4d9c-aff1-e63b02467303)

---

### Part 2: Get True Labels and Predictions

![Part 2](https://github.com/user-attachments/assets/3b4f72eb-7ee5-4744-a0fd-7864522111d3)

---

### Part 3: Precision, Recall, F1-Score

![Part 3](https://github.com/user-attachments/assets/aa2a5b7a-9022-479f-b163-a4372b1b2a11)

---

### Part 4: Confusion Matrix

![Part 4](https://github.com/user-attachments/assets/87575b50-4364-48d4-8ff1-8eb23141e83e)

---

### Part 5: Receiver Operating Characteristic (ROC) Curve and Area Under the Curve (AUC) Score

![Part 5](https://github.com/user-attachments/assets/96b9fcd0-f3c1-417b-bea9-a1d5c5ee19a6)

---

### Part 6: Plot ROC Curve

![Part 6](https://github.com/user-attachments/assets/4cd3b61b-5f2b-42f2-b590-19ed3f13be18)

---

### Part 7: AUC Score (Overall)

![Part 7](https://github.com/user-attachments/assets/b104c24d-99b2-4e16-8220-fea7b3de80e2)

---

### Part 8: Precision, Recall, F1 Visualization

![Part 8](https://github.com/user-attachments/assets/1743d928-62b6-472f-94cf-731c700db24d)


## Activity 2: Model Interpretability using
Gradient-weighted Class Activation Mapping
(Grad-CAM) - Visualizing CNN Decisions Using
Grad-CAM for Explainable Image Classification

### PART 1: Load the Saved Model
<img width="862" height="693" alt="image" src="https://github.com/user-attachments/assets/0fafbf4f-5542-478d-8fa2-d8ab8674fe42" />

### PART 2: Load and Preprocess Test Image
<img width="614" height="181" alt="image" src="https://github.com/user-attachments/assets/92a54552-944b-448a-bc64-9e97c03fa2cd" />

### PART 3: Identify Last Convolutional Layer
<img width="861" height="379" alt="image" src="https://github.com/user-attachments/assets/07da9733-7bf7-433c-8e18-8a91636f68cf" />

### PART 4: Build Grad-CAM Function
<img width="425" height="159" alt="image" src="https://github.com/user-attachments/assets/b7d34642-8ee0-4fc7-bb21-a03450d447b1" />

### PART 5: Generate Heatmap
<img width="508" height="434" alt="image" src="https://github.com/user-attachments/assets/3bcd35e3-0c79-497b-9e22-be8dbdbcab30" />

### PART 6: Superimpose Heatmap on Original Image
<img width="453" height="453" alt="image" src="https://github.com/user-attachments/assets/616020e2-7931-4863-9ec5-66b69d893eb8" />

### PART 7: Interpret the Results
Based on my Grad-CAM heatmap and overlay results, I can observe that the activation values range from 0.4 to 1.0, with the brightest yellow regions concentrated in the center of the image — which is exactly where the plant and flower are located. The darker purple and teal regions represent the background edges, indicating low activation in those areas. In the Grad-CAM overlay, the cyan highlights are clearly focused on the flower blooms at the top of the plant, which are the most visually distinctive parts of the subject, while the pink background and the pot received significantly less activation.
Based on these observations, I can conclude that my model is learning properly. The heatmap shows that my CNN is correctly focusing on the flower and plant region rather than the background, which means it has successfully learned meaningful and relevant visual features to make its classification decision. The highlighted region corresponds to the correct object, not the background, and the heatmap is not scattered — indicating that my model has developed strong feature learning. The high activation specifically on the blooms suggests that my model identified the most class-discriminative features of the plant, confirming that the regularization techniques applied during training helped the model generalize and focus on the right areas of the image.









