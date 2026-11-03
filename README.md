# RAG with Unsloth Dynamic 4-bit Quantization

## Project Overview
This project implements a Retrieval-Augmented Generation (RAG) pipeline using Unsloth's 4-bit quantized Llama 3.2 3B Instruct model.

The system retrieves relevant information from an uploaded PDF document and generates context-grounded answers using the quantized language model.

## Technologies Used
- Python
- Google Colab
- Unsloth
- Llama 3.2 3B Instruct (4-bit)
- Sentence Transformers
- FAISS
- PyPDF

## Project Workflow
1. Load the Unsloth 4-bit quantized language model.
2. Upload and extract text from PDF documents.
3. Split extracted text into smaller chunks.
4. Generate embeddings using Sentence Transformers.
5. Store document embeddings in a FAISS vector index.
6. Retrieve relevant document chunks based on user queries.
7. Generate answers using the retrieved context and Llama 3.2.

## Model and Hardware
- Model: Llama 3.2 3B Instruct
- Quantization: 4-bit
- GPU: NVIDIA Tesla T4
- Total GPU Memory: 14.56 GB
- Observed Model GPU Memory Allocation: 2.53 GB

## Testing and Results

**Relevant Question Test:**  
The model successfully retrieved information about parametric and non-parametric memory from the uploaded research paper and generated an answer.

**Irrelevant Question Test:**  
When asked who won the FIFA World Cup in 2022, the model correctly responded that the provided context did not contain enough information.

## Repository Contents
- `Task_3_RAG_Unsloth_Dynamic_4bit.ipynb` — Google Colab implementation notebook.
- `README.md` — Project documentation.

## How to Run
1. Open the notebook in Google Colab.
2. Select a GPU runtime.
3. Install the required libraries.
4. Upload your own PDF document.
5. Run the notebook cells in order.
6. Ask questions about the uploaded document.

## Learning Outcomes
- Understanding Retrieval-Augmented Generation.
- Working with 4-bit quantized language models.
- Building semantic search using embeddings.
- Implementing vector search with FAISS.
- Generating context-grounded LLM responses.

## Author
Kainat Zafar

GitHub: https://github.com/066300kainat
