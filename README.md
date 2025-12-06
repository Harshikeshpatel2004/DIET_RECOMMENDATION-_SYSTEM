# DIET_RECOMMENDATION_SYSTEM

## 🥗 Overview  
**DIET_RECOMMENDATION_SYSTEM** is a full-stack application (backend + frontend) that recommends personalized diet plans based on user inputs (e.g. age, weight, height, goals, dietary preferences). It uses machine learning / nutrition-logic to suggest foods/meals appropriate to the user’s requirements. The project consists of a user-friendly frontend (built with Streamlit) and a backend API (built with FastAPI) that generates recommendations.

## ✅ Features  
- Accepts user parameters (e.g. age, weight, height, dietary preferences, goals) to compute a suitable diet plan.  
- Supports multiple diet goals (e.g. weight-loss, weight-gain, maintenance) — configurable as per user needs.  
- Allows preference-based filtering (e.g. vegetarian / non-vegetarian, caloric limits, macro-nutrient constraints).  
- Clean separation of backend (API) and frontend (UI), making it easy to extend or integrate with other systems.  
- Option to export or display detailed meal plans (breakfast/lunch/dinner or customised meals).  

## 📁 Project Structure  
/
├── FastAPI_Backend/ # Backend API logic
├── Streamlit_Frontend/ # Frontend UI built using Streamlit
├── Assets/ # (Optional) Images / static assets / data files
├── requirements.txt # Python dependencies
├── render.yaml # (Optional) Deployment config (e.g. for Render or other hosts)
└── README.md # Project documentation


## 🛠️ Setup and Installation  

### Prerequisites  
- Python 3.x  
- Recommended: Virtual environment (venv / conda)  
- Install dependencies  

### Installation & Running Locally  
```bash
# Clone the repository
git clone https://github.com/Harshikeshpatel2004/DIET_RECOMMENDATION-_SYSTEM.git
cd DIET_RECOMMENDATION-_SYSTEM

# (Optional) create and activate virtual environment
python -m venv venv
source venv/bin/activate     # On Windows: `venv\\Scripts\\activate`

# Install dependencies
pip install -r requirements.txt

# To run backend API
cd FastAPI_Backend
uvicorn main:app --reload

# To run frontend UI
cd ../Streamlit_Frontend
streamlit run app.py         # or the appropriate main file
