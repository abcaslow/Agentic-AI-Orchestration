Subject: RAG Notes
From: Unitedwithcode <unitedwithcode@gmail.com>
To: Unitedwithcode <unitedwithcode@gmail.com>
Messages: 1

--- Unitedwithcode <unitedwithcode@gmail.com> (Wed, 14 Oct 2026 13:54:14 -0400) ---
A RAG (Retrieval-Augmented Generation) system uses the dot product to
mathematically measure how similar a user's search query is to text chunks
stored in a knowledge base. [1, 2]

How It Works

 -

 Turning Text into Numbers: The RAG system converts the user's question
 and all database documents into embeddings (long lists of numbers, or
 vectors, that capture semantic meaning). [1, 2]

 -

 Multiplying and Adding: The system calculates the dot product by
 multiplying matching numbers from the query vector and a document vector,
 then adding the totals together. [1]

 -

 Scoring Relevance: A higher dot product score means the vectors point in
 a similar direction, indicating that the text chunk matches the meaning of
 the user's question. [1, 2]

 -

 Retrieving Context: The system sorts these scores, pulls the top
 matching text chunks, and feeds them to a Large Language Model (LLM) to
 ground its final answer. [1, 2]

Key Considerations

 -

 Magnitude Bias: The raw dot product is affected by both the direction
 (meaning) and the length (magnitude) of the vectors. If a document is
 very long, its vector might score high simply due to its size rather than
 true relevance. [1, 2]

 -

 Normalization Fix: To fix this, many RAG pipelines normalize all vectors
 to a length of 1. When vectors are normalized, the dot product becomes
 mathematically identical to cosine similarity, safely comparing meaning
 purely by angle. [1, 2, 3]

How It Works in a RAG Pipeline

• Vector Conversion: RAG systems turn text documents and user search
queries into long lists of numbers called embeddings (vectors) using an AI
model.

• The Math: The dot product multiplies matching coordinates of two vectors
together and adds up the totals.

• The Match: During a search, the system computes the dot product between
the user's query vector and the stored document vectors. Higher scores mean
the content matches the query better.

The Shortcut with Normalized Vectors

• Normalized Data: If all vectors are scaled to a length of one
(normalized), the dot product mathematically equals cosine similarity.

• Speed: Vector databases use this shortcut because calculating a pure dot
product on normalized vectors is faster than running full angular
trigonometry calculations.

[image: image.png]

1) ARXIV ACADEMIC PAPER DATASET (AAPD) The AAPD dataset is a large dataset
for MLTC. It consists of 55,840 abstracts of papers about computer science
from Arxiv.1 An academic paper may have multiple subjects, and there are 54
subjects in total.

[image: image.png]

file:///C:/Users/bruce.caslow/Downloads/A_Hybrid_BERT_Model_That_Incorporates_Label_Semantics_via_Adjustive_Attention_for_Multi-Label_Text_Classification.pdf
