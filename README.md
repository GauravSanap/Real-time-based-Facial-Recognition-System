Real-time Facial Recognition System
<br>
Overview
This project implements a real-time facial recognition system using Python and various libraries such as OpenCV, NumPy, Tkinter, and face_recognition. The system allows users to add new faces to the recognition database, capture details associated with each face, and then recognize and display information about recognized faces in real-time.
<br>

Key Components
1. Add Person (addPerson.py)
Captures facial images using the computer's camera.
Utilizes OpenCV for real-time video stream processing.
Allows users to add details for the captured face, including name, age, and sex.
Saves captured images and associated details in the "People" directory.
Dependencies: OpenCV, NumPy, Tkinter
2. Add Records (addRecord.py)
Provides a Tkinter-based graphical user interface for adding details to the captured faces.
Saves the entered details in a JSON file ("Records.json").
Dependencies: Tkinter, json
3. Simple Face Recognition (simpleFaceRecord.py)
Implements face recognition using the face_recognition library.
Loads face encodings of known faces from the "People" directory.
Detects and recognizes faces in real-time video streams.
Dependencies: face_recognition, OpenCV, NumPy
4. View Details (viewDetails.py)
Displays details (name, age, sex) of recognized faces.
Fetches details from the "Records.json" file based on the recognized face's name.
Provides a Tkinter-based interface for displaying details.
Dependencies: Tkinter, json
5. Main (main.py)
Main script to launch the project.
Provides a Tkinter-based interface with options to add a new face and recognize faces.
Dependencies: Tkinter
Getting Started
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/real-time-facial-recognition.git
cd real-time-facial-recognition
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Run the main script:

bash
Copy code
python main.py
Usage
Add a New Face:

Click the "Add Face" button to capture a new face.
Enter details such as name, age, and sex.
Click "Submit" to save the details.
Recognize Faces:

Click the "Recognize Face" button to start real-time face recognition.
Detected faces will be displayed along with their names.
Click on a recognized face to view its details.
Configuration
Customize the configuration parameters in the code, such as the recognition threshold, video source, and file paths.
Contributing
Contributions are welcome! Feel free to open issues or create pull requests.
License
This project is licensed under the MIT License - see the LICENSE file for details.
Acknowledgments
Special thanks to the developers of OpenCV, NumPy, Tkinter, and face_recognition for their fantastic libraries.
