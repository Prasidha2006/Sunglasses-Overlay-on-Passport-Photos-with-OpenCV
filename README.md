# Sunglasses-Overlay-on-Passport-Photos-with-OpenCV

##  Project Overview
This project demonstrates how to overlay a sunglass image onto a human face using image processing techniques in Python. It uses alpha blending and masking to seamlessly place sunglasses over the eye region.

---

##  Objectives
- Read and display images
- Work with alpha channels (transparency)
- Resize and align overlay images
- Apply masking and blending techniques
- Generate a realistic augmented image

---

##  Technologies Used
- Python
- openCV
- :contentReference[oaicite:1]{index=1}
- NumPy
- Matplotlib
- Jupyter Notebook

---

##  Project Structure
```
├── main_sunglass.ipynb # Main notebook
├── passport.JPG # Input face image
├── sunglass.png # Sunglass image (with alpha channel)
└── README.md
```
##  Output

###  Step 1: Original Face Image  
<img width="825" height="1024" alt="passport" src="https://github.com/user-attachments/assets/0bbf3ac6-b976-4cc3-9458-055199d3090e" />

 
###  Step 2: Sunglass Image  
<img width="941" height="941" alt="sunglass" src="https://github.com/user-attachments/assets/29827f70-0997-4950-bd42-6edc09e42cf2" />


###  Step 3: Mask Visualization  
<img width="1605" height="308" alt="image" src="https://github.com/user-attachments/assets/031b17a2-c7be-4fe8-818a-160340cba6c8" />


###  Step 4: Naive Output  
<img width="930" height="911" alt="image" src="https://github.com/user-attachments/assets/8b6c0342-b968-4679-8c45-6834dd238ffe" />
 

###  Step 5: Final Output (Blended)  
<img width="1382" height="804" alt="image" src="https://github.com/user-attachments/assets/6593c673-a39c-42dd-bf3c-dde4b961022a" />


##  How It Works

### 1. Load Images
- Face image is loaded using OpenCV
- Sunglass image is loaded with alpha channel

### 2. Resize Sunglasses
- Adjust dimensions to match the eye region

### 3. Extract Channels
- Separate:
  - RGB (color channels)
  - Alpha (mask)

### 4. Create Mask
- Convert alpha channel into 3-channel mask

### 5. Overlay Sunglasses
Two approaches:
- **Naive overlay** (direct replacement)
- **Mask-based blending** (smooth and realistic)

##  Key Concepts

- Image slicing (Region of Interest - ROI)
- Alpha blending
- Bitwise operations
- Mask creation
- Channel separation
