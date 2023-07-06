# Tiny But Mighty: A Benchmark Dataset for Triple Extraction From Unstructured Text
This work introduces a novel dataset specifically designed to evaluate KG construction techniques from unstructured text. Our dataset consists of a diverse collection of compound and complex sentences meticulously annotated by human annotators with potential triples (subject, verb, object). The annotations underwent further scrutiny by expert ontologists to ensure accuracy and consistency. For evaluation purposes, the proposed F-measure criterion offers a robust approach to quantify the relatedness and assess the alignment between extracted triples and the ground-truth triples, providing a valuable tool for evaluating the performance of triple extraction systems.
# Dataset Statistics


# Evaluation
-	Implemented Tools/Libraries:
  1.	SpaCy (SVO) Extraction Model
  2.	Stanford OpenIE Triple Extractor
  3.	GPT4 via ChatGPT Prompt


-	Evaluation Criteria:
  1.	Triple Mentions' Vector
  2.	Vector Similarity (Ground Truth VS Extracted Triple)

-	Similarity Measures:
  1.	Cosine Similarity
  2.	Jaccard Similarity
  3.	Fuzzy Similarity

-	Evaluation Framework:
  1.	Removing Similar Triples from Tools’ Output
  2.	Calculating Each triple’s similarity score with GT Triples and keeping the highest similarity
  THRESHOLDS

# Thresholds
  Amnesty (A)	Correct (1)	0.81 – 1.00
	Partially Correct	0.5 – 0.8
  Penalty (P)	Incorrect (0)	< 0.5
