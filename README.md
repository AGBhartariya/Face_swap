# Face Swapping Model Using Deep Learning

This project is a **Face Swapping Model** built using **Python**, **OpenCV**, and **Dlib** that performs seamless face-swapping by leveraging facial landmarks, triangulation, and image blending techniques.

---

## 🚀 Features
- Accurate **face detection** and **landmark extraction** using **Dlib**.
- Efficient triangulation for precise facial alignment.
- **Affine transformations** for accurate face mapping.
- Natural-looking output with **cv2.seamlessClone()**.
- Supports real-time or image-based face swapping.

---

## 🛠️ Tech Stack
- **Python 3.11**
- **OpenCV**
- **Dlib**
- **PIL (Python Imaging Library)**
- **NumPy**
- **Requests**

---

## 📂 Project Structure
```
face_swap_project/
│
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

## 📥 Installation

1. **Clone the Repository**
```bash
git clone https://github.com/yourusername/face_swap_project.git
cd face_swap_project
```

2. **Create a Virtual Environment**
```bash
python -m venv venv
source venv/bin/activate    # For Linux/Mac
venv\Scripts\activate       # For Windows
```

3. **Install Dependencies**
```bash
pip install -r requirements.txt
```

4. **Download Dlib Landmark Model**
```bash
wget 'https://github.com/tzutalin/dlib-android/raw/master/data/shape_predictor_68_face_landmarks.dat'
```

---

## 🔄 Usage

1. **Run the Application**
```bash
python app.py
```

2. **Input Images**
- Add your face images in the `/uploads` folder or provide direct URLs within the code.

3. **Output**
- The output image will be saved in the `/output` folder or displayed on screen, depending on your implementation.

---

## 📋 Example Code Snippet
```python
# Creating seamless clone of two faces
result = cv2.add(img2_head_noface, img2_new_face)
(x, y, w, h) = cv2.boundingRect(convexhull2)
center_face2 = (int((x + x + w) / 2), int((y + y + h) / 2))
seamlessclone = cv2.seamlessClone(result, img2, img2_head_mask, center_face2, cv2.NORMAL_CLONE)
```

---

## 🧪 Sample Output
Refer to the three screenshots attached....


## 🧩 Challenges Faced & Solutions
✅ **Landmark Mismatch:** Resolved using precise triangulation logic and optimized alignment.  
✅ **Blending Issues:** Improved results using **cv2.seamlessClone()** for natural-looking skin tone blending.  
✅ **Image Scaling Problems:** Ensured both images are resized uniformly for better accuracy.

---

## 📜 Future Improvements
- Adding **real-time face swapping** via webcam.
- Implementing **GAN-based blending** for improved visual quality.
- Introducing a **UI interface** for user-friendly interactions.

---

## 🤝 Contributing
Contributions are welcome! If you have ideas or improvements, feel free to create a pull request or raise an issue.

---

## 📄 License
This project is licensed under the **MIT License**.

---

## 📧 Contact
For queries, feel free to reach out:
- **Name:** Abhigyan Gopal Bhartariya
- **Email:** [your_email@example.com](mailto:abhigyangb27@gmail.com)
- **LinkedIn:** [Your LinkedIn Profile](www.linkedin.com/in/abhigyan-bhartariya-73267928a)

---

### ⭐ If you find this project helpful, don't forget to give it a star!



