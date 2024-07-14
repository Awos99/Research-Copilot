# Research Copilot with RAG Chat

Research Copilot is an interactive web application designed to assist with research tasks using advanced language models and semantic analysis. Built using Streamlit, it provides an intuitive interface for processing and analyzing text inputs to extract key topics, search academic databases, visualize relationships, and interact through a chat interface.

## Features

-   **Topic Extraction**:

    -   Input a description of your research topic.
    -   Extract five key topics using GEMINI 1.5 FLASH.

-   **Paper Search**:

    -   Search for relevant academic papers in the Semantic Scholar database based on the extracted topics.

-   **Network Graph**:

    -   Visualize the relationships between the found papers in a network graph to understand their connections and relevance.

-   **Chat Functionality**:
    -   Switch to the chat page to interact with the language model.
    -   Web scrape the found papers and chunk them for detailed analysis.
    -   Use Cohere Rerank and Command R for contextually enriched responses via Retrieval-Augmented Generation (RAG).

## Installation

1. **Clone the repository**:

    ```sh
    git clone https://github.com/Awos99/Research-Copilot.git
    cd Research-Copilot
    ```

2. **Install the required packages**:

    ```sh
    pip install -r requirements.txt
    ```

3. **Add API keys**:
    - Obtain API keys for the necessary services (GEMINI, Cohere, Semantic Scholar).
    - Create the following files in the root directory and add your keys:
        - `COHERE_KEY.txt`
        - `GEMINI_KEY.txt`
        - `S2_API_KEY.txt`

## Usage

1. **Run the Streamlit application**:

    ```sh
    streamlit run app.py
    ```

2. **Interact with the application**:
    - **Main Page**: Enter a description of your research topic and click "Process Text" to extract key topics.
    - **Sidebar Options**: Select various options to customize your research process (WIP).
    - **Visualization**: View the network graph of related papers.
    - **Chat Page**: Switch to chat mode to interact with the language model, scrape papers, and receive contextually enriched responses.

Please, try the app here:

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://research-rag.streamlit.app/)
