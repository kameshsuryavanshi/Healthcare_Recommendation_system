
# Personalized Healthcare Recommendation System using GenAI

## Overview

Personalized healthcare recommendations are crucial for enhancing patient outcomes by providing tailored medical advice based on individual symptoms and medical histories. This project introduces a novel pipeline utilizing **Retrieval-Augmented Generation (RAG)**, combining domain-specific embeddings, dense retrieval, and advanced generative AI capabilities to deliver precise, context-aware medical recommendations.

---

## Key Features

1. **Semantic Understanding with BioBERT**:
   - Leverages BioBERT embeddings to capture nuanced semantics in medical documents and user queries.

2. **Efficient Retrieval with FAISS**:
   - Utilizes FAISS indexing for high-speed similarity searches across large collections of medical texts.

3. **Generative Response with Google Gemini**:
   - Integrates Google Gemini to generate coherent, contextually relevant healthcare recommendations.

---

## Architecture

The framework comprises three main components:

1. **Embedding Module**:
   - Uses BioBERT, a domain-specific BERT variant, to encode medical texts and user queries into dense vectors.

2. **Retrieval Module**:
   - Implements FAISS for indexing and retrieving the most relevant medical documents based on user input.

3. **Generation Module**:
   - Employs Google Gemini for synthesizing responses from retrieved documents, ensuring context-aware and personalized advice.

---

## Benefits

- **Precision in Retrieval**: Domain-specific BioBERT embeddings ensure accurate matching of user queries with relevant medical documents.
- **Speed and Scalability**: FAISS indexing enables efficient handling of large datasets.
- **Enhanced Recommendations**: Google Gemini generates coherent and contextually meaningful responses.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/healthcare-recommendation-system.git
   cd healthcare-recommendation-system
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download pre-trained BioBERT weights:
   - Follow instructions from the [BioBERT repository](https://github.com/dmis-lab/biobert).

4. Set up Google Gemini API access:
   - Obtain API credentials from [Google Gemini](https://ai.google.com/gemini).
   - Add your credentials to the environment variables or a configuration file.

---

## Usage

1. **Data Preparation**:
   - Place medical text datasets in the `data/` directory.

2. **Run the Pipeline**:
   ```bash
   python main.py --query "Your medical query here"
   ```

3. **Output**:
   - The system retrieves the most relevant medical documents and generates a personalized healthcare recommendation.

---

## Evaluation

- **Metrics**:
  - Retrieval Precision: Measures the relevance of retrieved documents.
  - Response Quality: Assessed via BLEU and ROUGE scores.

- **User Feedback**:
  - Highlights the system's potential to enhance patient care by providing reliable, personalized medical advice.

---

## Future Work

- Incorporate real-time updates to the medical knowledge base.
- Extend support for multilingual queries.
- Explore integration with wearable health devices for continuous monitoring.

---

## Contributions

- **Developers**:
  - [Kamesh Suryavanshi](https://github.com/kameshsuryavanshi) - Lead Developer

- **Acknowledgments**:
  - [BioBERT](https://github.com/dmis-lab/biobert) for domain-specific embeddings.
  - [FAISS](https://github.com/facebookresearch/faiss) for efficient similarity search.
  - [Google Gemini](https://ai.google.com/gemini) for generative AI capabilities.

---


