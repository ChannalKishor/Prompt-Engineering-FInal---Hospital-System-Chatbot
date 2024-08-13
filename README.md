

# Health Hive - Hospital System Chatbot

## About
This project is the final submission for the course Prompt Engineering INFO7375 at Northeastern University, conducted under the guidance of Professor Nick Brown. The project showcases the practical application of advanced prompt engineering techniques, LLMs, and generative AI to solve real-world problems in the healthcare domain.

### Authors
 1. Adhyantini Bogawat - NUID: 002766612 | [LinkedIn](https://www.linkedin.com/in/adhyantini-bogawat/) 
 2. Chinmay Dharwad - NUID: 002771037 | [LinkedIn](https://www.linkedin.com/in/chinmay-dharwad-476092128/)
 3. Kishor Channal - NUID: 002737089 | [LinkedIn](https://www.linkedin.com/in/kishorchannal/)   

## Introduction to the Project and Its Objectives

This project involves building a sophisticated chatbot for a large hospital system, leveraging the latest advancements in generative AI, retrieval-augmented generation (RAG), and large language models (LLMs). The primary objective is to provide stakeholders with a tool that can answer both structured and unstructured queries about hospital data, patient experiences, physician details, and more, without the need for complex query languages or reports. This project integrates multiple technologies including LangChain, Neo4j, and FastAPI to create a powerful and scalable solution.

### Architecture
![enter image description here](https://realpython.com/cdn-cgi/image/width=2000,format=auto/https://files.realpython.com/media/Screenshot_2024-01-15_at_8.08.18_PM.fe16f8a318cc.png)

## Detailed Explanation of the Use Case

The chatbot is designed to meet the specific needs of a large hospital system in the United States. The stakeholders need more visibility into the ever-changing data collected by the hospital, allowing them to ask ad-hoc questions about various aspects like patient visits, physician performance, and hospital operations. The chatbot leverages generative AI and RAG by integrating LLMs with graph databases (Neo4j) to answer these queries. The LangChain framework is used to manage the complexity of the chatbot's operations, including the decision-making processes of an AI agent that determines the appropriate tool to answer each query.

Key use cases include:

-   Retrieving current wait times at hospitals.
-   Aggregating and summarizing patient reviews to identify trends.
-   Answering detailed financial queries related to insurance billing.
-   Providing dynamic responses to complex, multi-faceted questions using AI-driven Cypher queries on the Neo4j graph database.

## Key Features and Functionalities

-   **LangChain Integration:** The chatbot uses LangChain to manage interactions between the LLMs and other tools like vector databases and custom functions.
-   **Neo4j Graph Database:** The hospital system data is stored and queried using Neo4j, which allows for complex relationships and connections between different entities like patients, visits, and physicians.
-   **RAG (Retrieval-Augmented Generation):** The chatbot retrieves relevant data from both structured (SQL-like) and unstructured (free-text reviews) sources to generate accurate, contextually relevant responses.
-   **FastAPI Deployment:** The chatbot is served via a FastAPI endpoint, enabling asynchronous interactions and scalable deployments.
-   **Streamlit UI:** A user-friendly interface built with Streamlit allows stakeholders to interact with the chatbot in a conversational manner.

## Challenges Faced and How They Were Overcome

-   **Data Integration:** One of the significant challenges was integrating diverse data sources, including structured hospital data and unstructured patient reviews, into a coherent graph database. This was overcome by designing a robust ETL pipeline using Neo4j and Python, ensuring all data was properly formatted and indexed.
-   **Handling Asynchronous Requests:** To ensure scalability and responsiveness, the API was designed to handle asynchronous requests. This required careful management of network latencies and retries, which was addressed by implementing retry logic and optimizing the FastAPI deployment.
-   **Dynamic Query Handling:** The chatbot had to be flexible enough to handle both simple queries (e.g., current wait times) and complex queries requiring aggregation and summarization. This was achieved by using LangChain's chaining and agent functionalities to dynamically select the appropriate tool for each query.

## Conclusion and Future Scope

This project successfully demonstrates the integration of advanced AI techniques with practical, real-world applications in healthcare. The chatbot not only meets the current needs of the hospital system but also sets the stage for future enhancements. Potential areas for future work include:

-   **Enhanced NLP Capabilities:** Incorporating more advanced NLP techniques to better understand and process complex medical terminology.
-   **Expanded Data Sources:** Integrating additional data sources, such as real-time patient monitoring data, to provide even more comprehensive insights.
-   **Advanced Analytics:** Adding predictive analytics capabilities to forecast trends and identify potential issues before they arise.
