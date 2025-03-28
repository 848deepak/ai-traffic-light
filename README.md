# 🚦 AI-Driven Traffic Light System

**📌 Introduction**

The AI-Driven Traffic Light System is designed to optimize traffic flow using real-time camera feeds and AI-based analysis. The system dynamically adjusts traffic signal timings based on:
✅ Traffic density analysis
✅ Vehicle classification (cars, buses, emergency vehicles, etc.)
✅ Lane-wise congestion comparison
✅ Real-time adaptive signal control

The project aims to reduce traffic congestion, prioritize emergency vehicles, and improve overall road efficiency.

⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻

**🛠️ Features**
	•	Real-time traffic detection – Uses a camera feed to analyze road conditions.
	•	Vehicle classification – Differentiates between cars, trucks, ambulances, firetrucks, etc.
	•	Dynamic signal adjustment – Adjusts traffic light duration based on detected congestion.
	•	Emergency vehicle priority – Detects ambulances or firetrucks and gives them a green signal.
	•	Multi-lane comparison – Determines the most congested lane and optimizes light timing accordingly.

⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻


**🚀 Technologies Used**
	•	Python – Core programming language
	•	OpenCV – Image processing and real-time traffic detection
	•	YOLOv8 / TensorFlow – Object detection for vehicle classification
	•	NumPy & Pandas – Data handling and processing
	•	Flask / FastAPI – Backend for processing and communication
	•	Raspberry Pi (Optional) – Can be deployed on edge devices
	•	Arduino (Optional) – For physical signal control

⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻


**📂 Project Structure**

ai-traffic-light/
│── dataset/                      # Training data for vehicle detection  
│── models/                       # Pre-trained YOLOv8 models  
│── scripts/                      # Python scripts for processing  
│   ├── detect_traffic.py         # Detects vehicles and density  
│   ├── classify_vehicles.py      # Identifies vehicle types  
│   ├── adjust_signal.py          # Algorithm for traffic light control  
│── app.py                        # Main entry point (Flask API)  
│── requirements.txt              # Python dependencies  
│── README.md                     # Project documentation  



⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻


**🛠️ Installation & Setup**

🔹 1. Clone the Repository

git clone https://github.com/848deepak/ai-traffic-light.git
cd ai-traffic-light

🔹 2. Install Dependencies

Ensure you have Python installed, then run:

pip install -r requirements.txt

🔹 3. Run the AI Traffic Detection Model

python scripts/detect_traffic.py

🔹 4. Start the Backend Server

python app.py

🔹 5. Connect to a Camera Feed

By default, the script will use the system webcam. To use an external camera:

python scripts/detect_traffic.py --source 1  # Change 1 to the correct camera ID



⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻


**🎯 How It Works**
	1.	Traffic Detection – Captures video feed and detects vehicles in each lane.
	2.	Vehicle Classification – Identifies vehicle types (cars, buses, emergency vehicles, etc.).
	3.	Traffic Density Analysis – Calculates congestion levels for each lane.
	4.	Signal Adjustment – Dynamically modifies green light durations based on congestion data.
	5.	Emergency Vehicle Detection – If an ambulance or firetruck is detected, it gets priority.

⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻


**📡 Deployment Options**

✅ Local System – Runs on a laptop or desktop.
✅ Raspberry Pi – Can be deployed at intersections for real-world usage.
✅ Cloud-Based – Can integrate with a cloud API for large-scale traffic management.

⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻


**📬 Contribution Guidelines**
	1.	Fork the repository and create a new branch for your changes.
	2.	Write clean, well-documented code.
	3.	Ensure compatibility – Test before pushing any changes.
	4.	Use descriptive commit messages – Example: "Added emergency vehicle detection logic"
	5.	Submit a pull request (PR) once your changes are ready.

⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻


**📜 Future Enhancements**

🔹 Integration with IoT sensors for real-time road condition updates.
🔹 Predictive analytics using machine learning to optimize traffic flow in advance.
🔹 Mobile app for live traffic updates and emergency alerts.
🔹 Smart city integration to communicate with public transport and smart signals.

⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻


**📝 Contact**

For any issues, reach out to Deepak Pandey at deepakpandey911494@gmail.com.

🚀 Let’s build a smarter traffic management system together!
