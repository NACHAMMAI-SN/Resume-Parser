# Resume-Parser
In order to assess resumes according to their technical abilities and credentials, this project creates a resume parser and classifier using machine learning techniques. Text extraction from multiple document formats (DOCX and PDF), text preprocessing, feature extraction, and classification using three distinct models—Decision Tree, Logistic Regression, and Random Forest—are the primary parts of the code.

IMPORTANT  ACTIONS :

●	Text Extraction : 	To ensure compatibility with various resume formats, the code offers routines to extract text from DOCX and PDF files.

●	Text Preprocessing :	 To make the extracted text in a format that is appropriate for analysis, preprocessing techniques such as tokenization, stopword removal, lemmatization, and cleaning are applied.

●	Feature extraction : 	To improve the classification model, more features are extracted, such as text length and the existence of particular technical skills.

●	TF-IDF Vectorization :	 Using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization, the resumes are converted into numerical representations that enable efficient comparison and analysis.


Model training and evaluation :

'Accepted' or 'Rejected' resumes make up the dataset, which is divided into training and testing sets for the purpose of model training and evaluation. The dataset is used to train and assess the Decision Tree Classifier, Random Forest, and Logistic Regression classifiers. Accuracy scores and classification reports are generated for each model.

Resume Classification :	Using the learned models, the code preprocesses and classifies resumes that users upload. For ease of interpretation, the decision tree visualisation is presented with the anticipated classifications.

Job Recommendation :	By computing the cosine similarity between the resume and job descriptions, the algorithm also suggests appropriate job listings based on the abilities gleaned from the resumes.

Output : 

The forecasts are downloaded and stored in a CSV file for additional examination or analysis.

Insights on candidate qualifications and possible job matches are provided by this project, which showcases the automated resume screening process using machine learning and natural language processing techniques.

