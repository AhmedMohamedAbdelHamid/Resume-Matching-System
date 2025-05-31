# Resume-Matching-System

An intelligent resume matching system that leverages Natural Language Processing and Machine Learning to automatically match candidates with job descriptions. This system processes resume text, extracts key features, and recommends the best-fit candidates for specific job roles.

## Project Overview

This project automates the resume screening process by:
- **Reducing manual effort** in candidate evaluation
- **Improving accuracy** of candidate-job matching
- **Leveraging NLP techniques** for semantic understanding
- **Providing ranked recommendations** for recruiters

## Dataset

- **Size**: 962 resumes across 25 job categories
- **Key Categories**:
  - Data Science (43)
  - HR (46)
  - Java Developer (37)
  - Business Analyst (37)
  - DevOps (28)
  - Network Security (25)

**Text Characteristics**:
- Average character count: ~6,000
- Average word count: ~1,000
- Range: 500 - 15,000 characters

## Technical Architecture

### Text Preprocessing Pipeline
1. **Normalization**: Remove accents and special characters
2. **Cleaning**: Strip numbers, punctuation, and non-alphabetic characters
3. **Tokenization**: Split text into individual words
4. **Lemmatization**: Reduce words to root forms
5. **Stopword Removal**: Filter out common words

**Impact**: ~30% reduction in word count while preserving semantic meaning

### Feature Extraction Methods

#### 1. TF-IDF Vectorization
- **Dimensions**: 3,000-dimensional document vectors
- **Top Terms**: experience, project, data, development, skills, python, machine learning, analysis
- **Purpose**: Capture term importance across documents

#### 2. Named Entity Recognition (NER)
Extracts key entities:
- **PERSON**: Candidate names
- **ORG**: Companies, universities
- **DATE**: Employment durations
- **GPE**: Geographic locations

#### 3. Keyphrase Extraction (YAKE)
Domain-specific term identification:
- **Data Science**: machine learning, predictive modeling, neural networks
- **HR**: recruitment process, employee engagement, performance management
- **DevOps**: cloud infrastructure, CI/CD pipelines, Kubernetes

## Matching Algorithms

### Similarity Methods

| Method | Approach | Key Features |
|--------|----------|--------------|
| **TF-IDF** | Text overlap | Fast computation, keyword-based |
| **BERT** | Semantic meaning | Context understanding, deep learning |
| **Hybrid** | Combined model | TF-IDF (60%) + BERT (40%) |

### Classification Models

| Model | Accuracy | Key Strengths |
|-------|----------|---------------|
| **Random Forest** | 100% | Best overall performance, robust |
| **Logistic Regression** | 100% | Fast inference, interpretable |
| **Naive Bayes** | 56% | Handles sparse data efficiently |

**Top Predictive Features**:
1. TF-IDF similarity score
2. Resume length
3. Keyword overlap count

### Job Description:
> "Senior Data Scientist with expertise in Python, machine learning, and cloud platforms. Experience with big data technologies preferred."

### Top Match:
- **Category**: Data Science
- **Similarity**: 0.87 (Hybrid)
- **Suitability**: Good Fit (92% probability)
- **Preview**: "Data scientist with 5+ years experience developing machine learning models in Python. AWS Certified. Led a team to deploy scalable ML solutions on cloud platforms..."

### Runner-Up Matches:
1. **DevOps** - Similarity: 0.79, Suitability: 85%
2. **Business Analyst** - Similarity: 0.72, Suitability: 78%

## Key Findings

1. **Hybrid Approach**: Combining TF-IDF and BERT provided the most accurate matching (60% TF-IDF + 40% BERT)
2. **Feature Importance**: Resume length and keyword density were critical predictors
3. **Model Performance**: Random Forest emerged as the most reliable classifier
4. **Scalability**: System can be extended to include more categories with minimal adjustments

## Future Enhancements

- [ ] Incorporate more job categories for broader applicability
- [ ] Fine-tune BERT model with domain-specific data
- [ ] Develop interactive web interface for recruiters
- [ ] Add multi-language support
- [ ] Implement real-time matching capabilities
- [ ] Add skill-gap analysis features

## Applications

- **Automated resume screening** for HR departments
- **Candidate ranking systems** for recruitment platforms
- **Skill-gap analysis** for workforce development
- **Talent matching** for freelance platforms

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Team

- **Ahmed Mohamed Abdelhamid** - 221011073
- **Omar Khalid** - 221002374
- **Ahmed Mohamed Hamimi** - 221011417

**Course**: IN321 Natural Language Processing  
**Institution**: Arab Academy for Science, Technology & Maritime Transport  
**Instructor**: Prof. Hanafy  
**Teaching Assistant**: Eng. Alia El Hefny

## Contact

For questions or collaboration opportunities, please reach out to the team members or create an issue in this repository.

---

⭐ **Star this repository if you find it helpful!** ⭐
