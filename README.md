
# Insight Attendance - Smart Face Recognition Attendance System 🎓📸

An advanced, automated attendance management system that leverages real-time facial recognition, computer vision, and cloud integration to transform traditional and online educational environments.

## 📌 Project Overview

**Insight Attendance** is designed to streamline the attendance-taking process using facial recognition. It not only automates roll calls but also captures student engagement levels and ensures accuracy through advanced machine learning algorithms and real-time database updates via Firebase.

## 🚀 Features

- 🔍 **Real-Time Face Detection & Recognition**
- ☁️ **Firebase Integration** (Realtime Database & Cloud Storage)
- 🕒 **Threshold-Based Attendance Logic**
- 🧠 **Machine Learning-Based Face Encodings**
- 💻 **Tkinter GUI and OpenCV-Based User Interface**
- 📊 **Excel Sheet Export of Attendance Logs**
- 🔐 **Secure Data Handling with Consent-Based Storage**
- 🔄 **Continuous Learning & Performance Tracking**
- 📡 **Supports Remote Learning via Webcam**
- 🧩 **API-ready architecture for third-party integration**

## 🛠️ Technologies Used

- **Programming Language**: Python
- **Libraries**: 
  - `OpenCV`, `cvzone`, `face_recognition`, `dlib`, `numpy`, `pickle`
  - `firebase_admin`, `datetime`, `tkinter`, `os`, `pandas`
- **Tools & Platforms**:
  - Jupyter Notebook
  - Firebase Realtime Database & Storage
  - Lucidchart (for system design & block diagrams)
  - Excel (for reporting)
  - Git & GitHub (for version control)

## 📷 System Flow (High Level)

1. **Registration**: Face data of students is captured and stored with their information.
2. **Detection**: System captures live feed, detects face using HOG/CNN, and encodes it.
3. **Recognition**: Matches the live encoding with stored data and updates attendance.
4. **Storage**: Records are stored securely in Firebase and exported to Excel for records.
5. **Feedback**: UI displays user-specific attendance info and status messages in real-time.

## 🧪 Testing & Validation

- Real-time detection and recognition tested under varying light conditions.
- Accuracy verified using Euclidean distance between encodings.
- Duplicate entry prevention via 30-second window logic.
- Attendance threshold set at minimum 60% of class time.

## 🔒 Privacy & Ethics

- All student data was collected with explicit consent.
- Data is deleted post-dissertation as per ethical guidelines.
- The system is compliant with data protection practices using Firebase security rules and local encryption.

## 🧠 Future Enhancements

- Support for multi-face detection.
- Liveness detection to avoid spoofing.
- Mobile app integration.
- Blockchain-based tamper-proof attendance logs.
- Expanded analytics dashboard with trend visualization.

## 📁 Project Structure

```
InsightAttendance/
├── encodings/                # Stored face encodings
├── Images/                   # Student face image dataset
├── servicekey.json           # Firebase admin credentials
├── main.py                   # Core application logic
├── register.py               # Student registration script
├── export_attendance.py      # Attendance export script
├── utils/                    # Utility functions
├── requirements.txt          # Python dependencies
└── README.md                 # Project documentation
```

## ⚙️ Installation

1. Clone this repo:
   ```
   git clone https://github.com/yourusername/Insight-Attendance.git
   cd Insight-Attendance
   ```

2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Configure Firebase:
   - Place your `servicekey.json` in the root directory.
   - Update the Firebase URL and storage bucket path in the script.

4. Run the app:
   ```
   python main.py
   ```

## 📊 Sample Output

- Real-time UI shows student name, ID, year, and attendance count.
- Auto-generates an Excel sheet (`Attendance_YYYY-MM-DD.xlsx`) with daily logs.
- Feedback messages: `Recognized`, `Already Marked`, `Unrecognized`.

## 📚 References

Project submitted as part of MSc at London Metropolitan University  
Supervisor: Pawel Gasiorowski  
Author: Smit Maheshbhai Jayani (ID: 22048422)  
Submission Date: 20th May, 2024

---

## 📬 Contact

Feel free to reach out for queries, collaboration, or suggestions:

**Email**: smit.jayani@example.com  
**LinkedIn**: [linkedin.com/in/smitjayani](https://linkedin.com/in/smitjayani)

---

> ⚠️ *This project is for academic demonstration only and should be used responsibly with proper consent for biometric data.*
> ⚠️ *If you want to use this project you need to have ethical approval form the students as the data of the students is confidential so we  have to follow the online rules and implement this project.* 
