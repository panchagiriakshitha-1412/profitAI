ProFit AI: Student Personalized Fitness & Diet Planner
ProFit AI is an intelligent web application designed to solve the "one-size-fits-all" problem in fitness. Built specifically for students, it leverages Machine Learning to provide budget-friendly nutrition and personalized workout protocols based on body composition and available resources.

🚀 The Problem Statement
Most fitness applications provide generic plans that ignore:

Individual Student Needs: Variability in BMI and body types.

Cultural Food Habits: Lack of regional/affordable food options.

Resource Constraints: Student budgets and limited workout equipment (Hostel vs. Gym).

✨ Key Features
AI Nutrition Engine: Uses K-Nearest Neighbors (KNN) to recommend meals based on specific protein goals and budget constraints.

Dynamic BMI Analysis: Real-time physiological assessment that categorizes users (Underweight, Healthy, Overweight).

Adaptive Exercise Protocols: Automatically switches between Hypertrophy (Muscle Gain) and Metabolic Conditioning (Fat Loss) based on BMI.

Context-Aware Workouts: Tailors routines for Hostel/Home (bodyweight) or Gym (equipment) environments.

Portable Reports: Users can download their AI-generated plan as a .txt file for offline use.

🛠️ Tech Stack
Language: Python 3.10+

Frontend: Streamlit (Responsive Web UI)

Machine Learning: Scikit-learn (KNN, StandardScaler)

Data Handling: Pandas & NumPy

Model Persistence: Pickle

📂 Project Structure
Plaintext
fitness/
├── data/
│   └── diet_data.csv          # Dataset of foods, costs, and protein
├── models/
│   ├── fitness_model.pkl      # Trained KNN Model
│   └── scaler.pkl             # Trained StandardScaler
├── app.py                     # Main Streamlit Application
├── train_ai.py                # Model Training Script
├── requirements.txt           # Project Dependencies
└── README.md                  # Project Documentation
⚙️ Installation & Usage
Clone the Repository:

Bash
git clone https://github.com/Siddhartha-raj-kotha/AICTE-BATCH-7-JAN-2026
cd ProFit-AI
Install Dependencies:

Bash
pip install -r requirements.txt
Train the AI Model:

Bash
python train_ai.py
Run the Application:

Bash
streamlit run app.py
🧠 AI Logic Breakdown
The project uses a hybrid approach:

Unsupervised Learning (KNN): To find the "Nearest Neighbors" in the nutritional dataset that satisfy the user's budget and protein requirements.

Rule-Based Inference: To map BMI values to specific rep ranges and exercise selections (e.g., lower BMI triggers hypertrophy logic; higher BMI triggers fat loss HIIT logic).

👤 Author
Panchagiri Akshitha - https://github.com/panchagiriakshitha-1412
Kotha Siddhartha Raj - https://github.com/Siddhartha-raj-kotha/ 
Marupaka Durga Bhavani - https://github.com/mdb0210
