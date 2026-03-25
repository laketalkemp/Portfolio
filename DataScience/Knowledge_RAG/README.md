# PML Knowledge Bot 🤖📚

A Retrieval-Augmented Generation (RAG) educational bot designed to answer questions strictly using content from the course textbook, <i>Personalized Machine Learning</i> by Dr. Julian McAuley.

Built for DSC 599: Teaching Methods at the University of California, San Diego.

## Architecture
<ul>
  <li> <b>Frontend:</b> Streamlit</li>
  <li> <b>Embeddings:</b> Local HuggingFace (<code>all-MiniLM-L6-v21</code> )</li>
  <li> <b>Vector Database:</b> ChromaDB</li>
  <li> <b>LLM:</b> Qwen 2.5 7B Instruct (via Hugging Face Serverless API)</li>
  <li> <b>Orchestration:</b> LangChain
</ul>

## How to Run Locally
<ol>
  <li> <b>Clone the repository:</b></li>
   
  ```bash
  git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
  cd your-repo-name
  ```
  <li> <b>Install the dependencies</b></li>
  
   ```pip install -r requirements.txt```
  <li> <b>Set your Hugging Face API Token:</b>
    
    export HUGGINGFACEHUB_API_TOKEN="your_token_here"
  <li><b>Launch the application:</b></li>
    
    streamlit run app.py
</ol>

## Deployment Notes (Streamlit Community Cloud)

If deploying to Streamlit Community Cloud:
<ol>
    <li>Connect your GitHub repository to Streamlit.</li>
    <li>Set the main file path to `app.py`.</li>
    <li>Go to Advanced Settings > Secrets in the Streamlit deployment dashboard and add your API key like this:</li>
  <code>HUGGINGFACEHUB_API_TOKEN = "your_token_here"</code>
</ol>    
