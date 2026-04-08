**🧠 Agentic RAG Pipeline with Contextual AI**

This project implements an end-to-end Retrieval-Augmented Generation (RAG) pipeline using Contextual AI, exploring how modern AI systems retrieve, refine, and generate grounded responses from external knowledge sources.

This work was developed by following and adapting concepts from the rag_techniques repository https://github.com/NirDiamant/rag_techniques. 

**🚀 Project Overview**

The aim of this project was to understand how to build more reliable AI systems by:

Retrieving relevant information from a datastore
Improving result quality using reranking
Generating grounded responses based on evidence
Reducing hallucinations
Evaluating output quality using automated metrics

Rather than focusing only on model outputs, this project explores the full pipeline behind real-world AI systems.

**⚙️ Pipeline Architecture**

The system follows a structured RAG workflow:

1. Datastore Creation
A datastore is created to store and manage documents
Acts as the knowledge base for retrieval
2. Document Parsing
Raw documents are processed into structured format
Ensures compatibility with retrieval and ranking steps
3. Retrieval
Relevant documents are fetched based on user queries
Forms the foundation of the RAG pipeline
4. Reranking
Retrieved documents are reordered using an instruction-following model
Improves relevance and prioritises higher-quality information
5. Grounded Generation
The model generates responses using only retrieved knowledge
Reduces hallucinations and improves factual accuracy
6. Evaluation (LMUnit)
Responses are evaluated for groundedness and quality
Helps assess reliability before deployment
🧪 Experiments & Observations

The project includes several practical experiments:

Comparing grounded vs non-grounded responses
Analysing the impact of reranking on retrieval quality
Testing behaviour with irrelevant knowledge
Evaluating the effect of avoid_commentary on outputs
📊 Key Insights
Reranking significantly improves relevance when multiple documents are retrieved
Grounded generation reduces unsupported or hallucinated answers
Poor or irrelevant knowledge negatively impacts output quality
Evaluation is essential for validating AI system performance

**🛠️ Technologies Used**
Python
Contextual AI API
Requests
Retrieval-Augmented Generation (RAG) concepts

**▶️ How to Run**
Clone this repository
Create a .env file in the project root:
API_KEY=your_api_key_here
Install dependencies:
pip install python-dotenv requests
Run the notebook:
agentic_rag_pipeline.ipynb

**🔐 API Key Security**

API keys are managed securely using environment variables and are not included in this repository.

**📌 Notes**

This project was developed as part of a learning exercise to explore modern RAG pipelines. The focus is on understanding system behaviour, design decisions, and limitations rather than production deployment.
