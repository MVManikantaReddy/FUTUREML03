# FUTUREML03 - Resume Screening System

**Author:** M.V. Manikanta Reddy  
**GitHub:** [MVManikantaReddy](https://github.com/MVManikantaReddy)  
**Internship:** Future Interns ML Task 03

## 📊 Task: Resume Candidate Screening
ML system to screen and rank resumes based on job role requirements.

## 🛠 Tech Stack
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![spaCy](https://img.shields.io/badge/spaCy-09A3D5?style=for-the-badge&logo=spacy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)

## 🚀 Setup
```bash
pip install -r requirements.txt
jupyter notebook resume_screening.ipynb
```

## 🎯 Features

- **Resume Parsing**: Extract text from resume documents using spaCy
- **Skill Extraction**: Automatically identify technical and soft skills from resumes
- **Job Matching**: Match resume skills against job description requirements using TF-IDF
- **Ranking Algorithm**: Rank candidates by cosine similarity score
- **Skill Gap Analysis**: Identify missing skills for each candidate
- **Visualizations**: Generate charts showing candidate rankings and skill matches

## 📊 Implementation Details

### Data Pipeline
1. **Synthetic Dataset Generation**: 50 realistic resumes + 1 Data Scientist job description
2. **Text Preprocessing**: Tokenization and cleaning using spaCy NLP
3. **Feature Extraction**: TF-IDF vectorization of job description and resumes
4. **Similarity Scoring**: Cosine similarity computation between resume and job vectors
5. **Ranking & Analysis**: Rank candidates and compute skill gaps

### Algorithm Flow
```
Job Description -> TF-IDF Vector
       |
       v
Resumes -> TF-IDF Vectors
       |
       v
Cosine Similarity Scores
       |
       v
Ranked Candidates (Top 5)
       |
       v
Skill Gap Analysis & Visualization
```

## 📈 Key Metrics

- **Match Percentage**: Resume skills / Job requirements (expressed as %)
- **Similarity Score**: Cosine similarity (0-1 scale, higher is better)
- **Top-3 Accuracy**: % of highly qualified candidates in top 3 positions
- **Target Accuracy**: 80%+ (achieved in demo)

## 🚀 Usage

Run the Jupyter notebook to execute the full pipeline:
```bash
jupyter notebook resume_screening.ipynb
```

The notebook demonstrates:
- Loading and displaying the job description
- Processing 50 synthetic resumes
- Screening 3 new test resumes in real-time
- Generating ranking and skill gap visualizations

## 📋 Results Sample

Top 5 ranked candidates for Data Scientist position:

| Rank | Candidate | Match % | Top Skills | Missing Skills |
|------|-----------|---------|-----------|----------------|
| 1    | Alice Chen | 92% | Python, ML, TF-IDF | Big Data Platforms |
| 2    | Bob Kumar | 87% | Python, Pandas, ML | Deep Learning, Cloud |
| 3    | Carol Smith | 85% | Python, Data Analysis | NLP, TensorFlow |
| 4    | David Patel | 78% | Python, Stats | ML Frameworks, Cloud |
| 5    | Eve Johnson | 72% | Data Viz, Python | ML, Advanced Stats |

## 📁 Project Structure

```
FUTUREML03/
├── resume_screening.ipynb    # Main Jupyter notebook
├── requirements.txt          # Python dependencies
├── README.md                 # This file
└── .gitignore               # Git ignore file
```

## 🔧 Dependencies

- Python 3.9+
- pandas: Data manipulation
- numpy: Numerical computations
- scikit-learn: ML tools and TF-IDF
- matplotlib: Data visualization
- seaborn: Statistical plots
- spacy: NLP for skill extraction
- jupyter: Interactive notebooks

## 💡 Future Enhancements

- [ ] Support for real resume PDF/DOCX parsing
- [ ] Multi-language resume screening
- [ ] Advanced NER for skill identification
- [ ] Deep learning models (BERT embeddings)
- [ ] Web interface for live screening
- [ ] Database integration for candidate storage
- [ ] Salary prediction based on skills

## 📚 Learning Outcomes

- Text preprocessing and NLP techniques
- Feature extraction and TF-IDF vectorization
- Similarity metrics (cosine similarity)
- Data visualization best practices
- Skill gap analysis methodology
- Business insights from ML systems

## 👤 Author

**M.V. Manikanta Reddy**
- GitHub: [MVManikantaReddy](https://github.com/MVManikantaReddy)
- Future Interns ML Task 03

---

*Last Updated: 2024 | This project is part of Future Interns ML internship program*
