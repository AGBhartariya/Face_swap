# Face Swapping Model Using Deep Learning

![Face Swap Demo](https://wallpapers.com/images/hd/shah-rukh-khan-classy-suit-xpxcz257rb1ple9l.jpg)

## 🚀 Project Overview
This project is a **Face Swapping Model** built using **Python**, **OpenCV**, and **Dlib**. It efficiently swaps faces between two given images while maintaining realistic blending using computer vision techniques.

The model leverages facial landmark detection, triangulation, affine transformation, and seamless cloning to achieve precise and natural-looking face swaps.

---

## 🧑‍💻 Features
✅ Accurate face landmark detection using **Dlib's 68 landmark predictor**  
✅ Efficient triangulation-based mapping for better facial structure alignment  
✅ Natural blending with **`cv2.seamlessClone()`** for realistic integration  
✅ Robust handling of complex face geometries and multiple face swaps  
✅ Flexible structure allowing easy extension for live video feeds or webcam integration  

---

## 📂 Project Structure
```
face_swap_project/
├── static/
│   ├── css/
│   │   └── style.css
│   ├── js/
│   │   └── script.js
│   └── uploads/
│
├── templates/
│   └── index.html
│
├── app.py
├── face_swap_model.py
├── requirements.txt
└── README.md
```

---

## 🔧 Installation Guide

### Step 1: Clone the Repository
```bash
git clone https://github.com/<YourGitHubUsername>/<RepositoryName>.git
cd <RepositoryName>
```

### Step 2: Install Dependencies
Install required packages from `requirements.txt`:
```bash
pip install -r requirements.txt
```

### Step 3: Download Dlib Landmark Model
Since Dlib's landmark model is large, download it using:
```bash
wget https://github.com/davisking/dlib-models/raw/master/shape_predictor_68_face_landmarks.dat
```
Place this file in your project directory.

### Step 4: Run the Project
For Google Colab:
```python
from google.colab import drive
drive.mount('/content/drive')
%cd /content/drive/MyDrive/<Your_Project_Folder>
```

For Local Environment:
```bash
python app.py
```

---

## 📋 Usage
1. Upload two face images for swapping.
2. The model will:
   - Detect facial landmarks using **Dlib**.
   - Perform triangulation and affine transformation to align features.
   - Use seamless cloning to merge faces naturally.
3. The final swapped image will be displayed and saved in the `/uploads` folder.

---

## 📷 Sample Images
| Original Image 1 | Original Image 2 | Swapped Output |
|:----------------:|:-----------------:|:---------------:|
| ![Image 1]("C:\Users\abhig\OneDrive\Pictures\Screenshots\Screenshot 2025-03-10 113858.png") | ![Image 2]("C:\Users\abhig\OneDrive\Pictures\Screenshots\Screenshot 2025-03-10 113909.png") | ![Result]("C:\Users\abhig\OneDrive\Pictures\Screenshots\Screenshot 2025-03-10 113925.png") |

---

## 🔎 Technical Details
- **Face Landmark Detection:** Utilizes `dlib.get_frontal_face_detector()` for face detection and `dlib.shape_predictor()` for facial landmark detection.
- **Triangulation & Warping:** Ensures each facial feature is aligned accurately for a smooth swap.
- **Seamless Cloning:** Uses OpenCV’s `cv2.seamlessClone()` to blend the swapped face naturally into the target image.

---

## 🧠 Challenges Faced & Solutions
🔹 **Alignment Issues:** Improved by refining bounding box detection and adjusting triangle mask dimensions.  
🔹 **Blending Artifacts:** Resolved by fine-tuning the seamless clone mask.  
🔹 **Image Download Errors:** Added exception handling for invalid URLs.  

---

## 💡 Future Enhancements
✅ Implement a **live webcam-based face swapping** feature.  
✅ Add a **user interface (UI)** for smoother interaction.  
✅ Incorporate **real-time face tracking** for enhanced performance.  

---

## 🤝 Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m "Add new feature"`).
4. Push to the branch (`git push origin feature-name`).
5. Open a Pull Request.

---

## 🏅 Credits
- **OpenCV** for computer vision functions.  
- **Dlib** for landmark detection.  
- **Python** for logic and data manipulation.  

---

## 📜 License
This project is licensed under the **MIT License**.

---

## 📬 Contact
Feel free to connect with me via [LinkedIn](https://www.linkedin.com/in/<YourProfile>) or email at `<your.email@example.com>` if you have any questions or suggestions!

