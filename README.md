# Sentiment_Analysis_Logisticregression

<h2>Resume Job Category Prediction</h2>

<p>This project focuses on classifying resumes into predefined job categories (e.g., Data Science, HR, Web Developer) using <b>Natural Language Processing (NLP)</b> techniques and a <b>Logistic Regression</b> classifier. The approach combines text preprocessing, feature extraction via TF-IDF, and supervised machine learning to achieve high accuracy.</p>

<hr>

<h2>Objective</h2>
<p>The main objective of this assignment is to build a machine learning model capable of automatically predicting the job category of a given resume based on its content. This can assist recruiters and HR teams in quickly filtering and categorizing resumes.</p>

<hr>

<h2>Dataset Description</h2>
<ul>
  <li><b>Dataset Name:</b> UpdatedResumeDataSet.csv</li>
  <li><b>Number of Records:</b> 962 resumes</li>
  <li><b>Columns:</b>
    <ul>
      <li><code>Category</code> – The job category label (e.g., Data Science, HR).</li>
      <li><code>Resume</code> – The raw text content of the resume.</li>
    </ul>
  </li>
</ul>

<hr>

<h2>Methodology</h2>
<ol>
  <li><b>Data Preprocessing</b>
    <ul>
      <li>Lowercasing and removal of special characters.</li>
      <li>Tokenization using spaCy.</li>
      <li>Stopword removal to eliminate non-informative words.</li>
      <li>Lemmatization to reduce words to their base form.</li>
    </ul>
  </li>
  <li><b>Feature Extraction</b>
    <ul>
      <li>Applied <b>TF-IDF Vectorization</b> with 5000 features to represent text numerically.</li>
    </ul>
  </li>
  <li><b>Model Building</b>
    <ul>
      <li>Used <b>Logistic Regression</b> as the classifier.</li>
      <li>Split data into training and test sets (80%-20%).</li>
    </ul>
  </li>
  <li><b>Evaluation</b>
    <ul>
      <li>Evaluated the model using <b>accuracy score</b>, achieving <b>99% accuracy</b> on test data.</li>
      <li>Generated a confusion matrix and classification report.</li>
    </ul>
  </li>
</ol>

<hr>

<h2>Key Results</h2>
<ul>
  <li>Achieved <b>99% accuracy</b> on test data.</li>
  <li>Correctly classified unseen resumes such as HR, Data Science, and Mechanical Engineer.</li>
  <li>Displayed top-3 category probabilities for better interpretability.</li>
</ul>

<hr>

<h2>Sample Prediction</h2>
<pre>
Input: "Full-stack web developer skilled in React, Node.js, MongoDB, and CI/CD."
Output:
Predicted category: Web Developer
Top-3 probabilities:
  Web Developer: 0.35
  Python Developer: 0.21
  Data Science: 0.09
</pre>

<hr>

<h2>Applications</h2>
<ul>
  <li>Automated resume screening for recruiters.</li>
  <li>Efficient job-role mapping for career portals.</li>
  <li>Enhancing applicant tracking systems with AI-based classification.</li>
</ul>

<hr>

<h2>Future Work</h2>
<ul>
  <li>Experiment with deep learning models like LSTM or BERT for better semantic understanding.</li>
  <li>Deploy the model as an API or web application for real-time resume classification.</li>
  <li>Enhance dataset diversity to cover more job roles.</li>
</ul>

<h2>Conclusion</h2>
<p>
This project successfully demonstrates how NLP techniques and machine learning can be combined to classify resumes into relevant job categories. 
Through thorough text preprocessing, TF-IDF vectorization, and the use of a Logistic Regression model, we achieved an impressive 99% accuracy on test data. 
The model performs well even on unseen resumes and provides top-3 probable categories for better interpretability. 
Future improvements such as deep learning models and deployment as a web service can make this solution production-ready and highly useful for automated recruitment systems.
</p>
