# Big-Data-CSL7110-Assignment

## Overview
This project demonstrates distributed data processing using **Hadoop (HDFS + MapReduce)** and **Apache Spark (PySpark)** on Project Gutenberg text files.

---
## Hadoop

**Q1–Q6:**  
- Installed and configured Hadoop in WSL Ubuntu.
- Created HDFS directories.
- Uploaded dataset to HDFS.
- Verified file structure and replication.
- Performed basic HDFS commands (ls, rm, copyFromLocal).

**Q7:**  
- Implemented `WordCount.java`.
- Compiled and created JAR file.
- Executed MapReduce job on HDFS.
- Retrieved output and verified word counts.

**Q8:**  
- Verified HDFS replication factor (applies to file blocks, not directories).  

**Q9:**  
- Analyzed performance using different input split sizes.  
- Observed trade-off between task overhead and parallelism.  

---

## Spark (PySpark)

**Q10 — Metadata Extraction:**  
- Extracted title, author, release date, language, and year using regex.  
- Computed books per year and basic statistics.  

**Q11 — TF-IDF & Similarity:**  
- Preprocessed text and computed TF-IDF vectors.  
- Calculated cosine similarity between books.  
- Discussed scalability of pairwise comparisons.  

**Q12 — Author Influence Network:**  
- Built directed graph (author1 → author2) based on publication gap:  
  `0 < (year_B - year_A) ≤ X`  
- Compared:
  - X = 3 → 10853 edges  
  - X = 5 → 12241 edges  
  - X = 10 → 14460 edges  
- Selected X = 5 as balanced representation.  
- Computed in-degree and out-degree.  

---

## Technologies
Hadoop, HDFS, MapReduce (Java), Apache Spark 3.5.1(PySpark), Jupyter Notebook, WSL Ubuntu.

---

## Conclusion
The assignment demonstrates distributed storage, MapReduce processing, Spark-based text analytics, TF-IDF similarity, and scalable graph modeling.
