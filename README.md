# AI-Powered Medical Knowledge Graph

## Overview
This project implements an **AI-powered knowledge graph** for medical query analysis and disease recommendation. It leverages **Neo4j** for storing medical relationships, **NLP** for symptom extraction, and **graph embeddings (Node2Vec)** for intelligent recommendations.

## Features
- **Symptom-based Disease Prediction**: Users can input symptoms and get possible disease predictions.
- **Knowledge Graph Construction**: Uses **Neo4j** to store and query relationships between diseases, symptoms, and precautions.
- **Natural Language Processing (NLP)**: Extracts relevant symptoms from user queries using a BERT-based model.
- **Graph Embeddings (Node2Vec)**: Enhances disease-symptom relationship understanding for improved recommendations.
- **REST API (Flask)**: Backend service for handling user requests and querying the knowledge graph.
- **Interactive UI**: Simple web-based interface for user interaction.

## Tech Stack
- **Backend**: Python, Flask, Neo4j
- **Database**: Neo4j (Graph Database), SQLite (User Sessions)
- **Machine Learning**: NLP (BERT), Node2Vec (Graph Embeddings)
- **Frontend**: HTML, CSS, JavaScript (Flask-based UI)

## Installation & Setup
### Prerequisites
Ensure you have the following installed:
- Python 3.12+
- Neo4j Database
- Flask (`pip install flask`)
- Required dependencies (`pip install -r requirements.txt`)

### Steps to Run the Project
1. **Clone the Repository**
   ```sh
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   ```
2. **Install Dependencies**
   ```sh
   pip install -r requirements.txt
   ```
3. **Start Neo4j** (Ensure the database is running)
4. **Run the Data Ingestion Script**
   ```sh
   python data_ingestion.py
   ```
5. **Start the Flask API**
   ```sh
   python app.py
   ```
6. **Access the Web UI**
   Open `http://127.0.0.1:5000/` in your browser.

## Usage
- Enter symptoms in the UI or via API endpoint (`/predict`)
- The system will analyze the input and return possible diseases
- Precautions and descriptions for each disease are displayed

## API Endpoints
| Endpoint | Method | Description |
|----------|--------|-------------|
| `/predict` | POST | Accepts symptoms and returns disease predictions |
| `/history` | GET | Retrieves user query history |
| `/graph` | GET | Visualizes the medical knowledge graph |

## Challenges & Limitations
- **Limited dataset availability** affects the accuracy of rare disease predictions.
- **High computational requirements** for Node2Vec graph embeddings.
- **NLP complexity** in processing multilingual symptom queries.

## Future Improvements
- **Integration with Large Real-time Datasets** for better personalization.
- **Enhanced AI explanations** for better transparency.


## Contributors
- VELMURUGAN
- VIKASH VARDHAN
- DINESHKUMAR
- INDIRA NIVAS
