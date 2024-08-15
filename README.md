

# Health Hive - Hospital System Chatbot

## About
This project is the final submission for the course Prompt Engineering INFO7375 at Northeastern University, conducted under the guidance of Professor Nick Brown. The project showcases the practical application of advanced prompt engineering techniques, LLMs, and generative AI to solve real-world problems in the healthcare domain.

### Youtube Video Link

### Project Setup
1. Set up a Neo4J AuraDB instace. 
2. Create a .env file with the following environment variables

```
NEO4J_URI=<YOUR_NEO4J_URI>
NEO4J_USERNAME=<YOUR_NEO4J_USERNAME>
NEO4J_PASSWORD=<YOUR_NEO4J_PASSWORD>

OPENAI_API_KEY=<YOUR_OPENAI_API_KEY>

HOSPITALS_CSV_PATH=/data/hospitals.csv
PAYERS_CSV_PATH=/data/payers.csv
PHYSICIANS_CSV_PATH=/data/physicians.csv
PATIENTS_CSV_PATH=/data/patients.csv
VISITS_CSV_PATH=/data/visits.csv
REVIEWS_CSV_PATH=/data/reviews.csv
EXAMPLE_CYPHER_CSV_PATH=/data/example_cypher.csv

CHATBOT_URL=http://host.docker.internal:8000/hospital-rag-agent

HOSPITAL_AGENT_MODEL=gpt-4o-mini
HOSPITAL_CYPHER_MODEL=gpt-4o-mini
HOSPITAL_QA_MODEL=gpt-4o-mini

NEO4J_CYPHER_EXAMPLES_INDEX_NAME=questions
NEO4J_CYPHER_EXAMPLES_NODE_NAME=Question
NEO4J_CYPHER_EXAMPLES_TEXT_NODE_PROPERTY=question
NEO4J_CYPHER_EXAMPLES_METADATA_NAME=cypher
```

3. Install Docker Compose
4. Open a terminal and run 
   ``` docker-compose up --build ```

5. After the container finishes building, you will be able to access the application at http://localhost:8501/

### Authors
 1. Adhyantini Bogawat - NUID: 002766612 | [LinkedIn](https://www.linkedin.com/in/adhyantini-bogawat/) 
 2. Chinmay Dharwad - NUID: 002771037 | [LinkedIn](https://www.linkedin.com/in/chinmay-dharwad-476092128/)
 3. Kishor Channal - NUID: 002737089 | [LinkedIn](https://www.linkedin.com/in/kishorchannal/)   