# Information Retrieval Document Search Engine 
## **BERT Search Engine**

### **Project Description**
The BERT Search Engine uses **pre-trained BERT embeddings** to provide a semantic-based document retrieval system. Unlike traditional keyword-based methods, it understands the context and relationships between words, making it highly effective for complex and ambiguous queries.

### **Features**
- **Semantic Understanding**: Leverages BERT embeddings to capture the meaning of text.
- **Contextual Search**: Finds documents relevant to the context of the query, not just keyword matches.
- **Ranking by Similarity**: Uses cosine similarity to rank documents based on their semantic proximity to the query.

### **Implementation**
1. **Text Preprocessing**:
   - Tokenizes documents and queries using a BERT tokenizer.
   - Converts text into embeddings using a pre-trained BERT model.

2. **Embedding Storage**:
   - Generates and stores document embeddings in a vector database or file system for efficient retrieval.

3. **Query Processing**:
   - Processes user queries into embeddings.
   - Computes similarity between the query embedding and document embeddings.

4. **Result Ranking**:
   - Ranks results based on cosine similarity scores.

---

## **TF-IDF Search Engine**

### **Project Description**
The TF-IDF Search Engine is a traditional vector space retrieval system. It uses **Term Frequency-Inverse Document Frequency (TF-IDF)** to assign weights to terms and ranks documents based on their similarity to user queries.

### **Features**
- **Keyword Matching**: Focuses on exact term matching within documents.
- **Efficient Indexing**: Utilizes an inverted index for fast term lookups.
- **Ranking by Relevance**: Computes similarity using cosine similarity on TF-IDF vectors.
- **Performance Optimization**: Includes index elimination and champion lists to enhance response time.

### **Implementation**
1. **Text Preprocessing**:
   - Tokenizes and normalizes text.
   - Removes stop words and performs stemming or lemmatization.

2. **Index Construction**:
   - Builds an inverted index to store term frequencies and document mappings.
   - Calculates TF-IDF weights for each term.

3. **Query Processing**:
   - Converts user queries into TF-IDF vectors.
   - Computes cosine similarity between query and document vectors.

4. **Result Ranking**:
   - Returns a ranked list of documents based on relevance scores.
