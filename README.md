# Charan Sai Neelisetty

Machine learning & data science engineer · Student · Ongole, India

Personal portfolio website. A single static page (`index.html`) with no build step and no dependencies apart from the EB Garamond web font.

- **Live site:** https://charan7sai.github.io/Portfolio/
- **Run locally:** open `index.html` in a browser, or run `python -m http.server 8124` in this folder and visit http://localhost:8124

---

## About

I am an undergraduate in Computer Science (AI/ML) at Manipal University Jaipur, and concurrently in the B.S. Data Science programme at IIT Madras. I build machine learning systems end to end: collecting the data, setting up an honest evaluation, training the model, and shipping it as something people can actually use.

My recent work spans probabilistic forecasting, computer vision, cross modal recommendation, large scale entity resolution and ML for supply chain security. I am a Microsoft Certified Fabric Data Engineer Associate (DP-700).

---

## Experience

### Cybersecurity AI/ML Research Intern
*SwiftSafe Cybersecurity Technologies · Remote · Mar – Jul 2026*

- Researched ML driven threat detection for CI/CD software delivery pipelines, analysing threats and recommending security measures and models that strengthened detection coverage.
- Improved the datasets behind threat classification research and turned findings into actionable recommendations with the research team.

### Machine Learning Intern
*Intern Vision Technology (DPIIT Recognised) · Remote · Dec 2025 – Feb 2026*

- Delivered an end to end ML project on real time industrial data in a three month, mentor led programme.
- Owned preprocessing, model development, evaluation and deployment. Rated commendable by the founders.

---

## Projects

### [Powercast](https://github.com/Charan7sai/Powercast) · Day ahead power price forecasting & battery trading
*Oct 2026 · LightGBM, conformal prediction, SciPy, SHAP, FastAPI, Docker, Streamlit · [Live demo](https://powercast-price-trading.streamlit.app/)*

- Forecasts 24 hourly electricity prices for three European markets from 8 years of price and weather data, using only information available before the noon auction.
- A global quantile LightGBM beats the LEAR academic benchmark by 5.5% MAE over 663 walk forward test days (Diebold–Mariano p < 0.001).
- Conformalised quantile regression lifts 80% interval coverage from 60% to 79.8%.
- LP optimised battery trading on the forecasts captures 93.9% of perfect foresight profit, against 88.5% for a naive forecast.

### [Vibe Embeddings](https://github.com/Charan7sai/vibe-embeddings) · Cross modal music & film recommender
*Jun – Oct 2026 · PyTorch, CLAP, Sentence-Transformers, Scikit-learn, FastAPI, Docker*

- Matches songs and films by mood across 2,189 songs and 2,992 films collected from public APIs.
- Built a ground truth benchmark from 1,107 official soundtrack songs across 310 films, after finding the baseline model performed at chance.
- Fusing audio text embeddings with a learned ridge projection moved the true match from the 48th percentile to the top 22%.
- Hubness correction widened coverage from 958 to 1,502 distinct recommended films.

### [Business Entity Resolution](https://github.com/Charan7sai/Amazon-ML-Challenge) · ML Challenge 2026
*Sep 2026 · LightGBM, rapidfuzz, sparse_dot_topn*

- CPU only pipeline over 1.73M entities and 9.97M records, scoring 0.9225 F0.5.
- Country partitioned sparse blocking cut 17 trillion candidate pairs to 26 million.
- LightGBM matcher on 26 string similarity features, with the threshold tuned directly on macro F0.5.
- A one to one assignment constraint lifted F0.5 from 0.812 to 0.9225.

### CrowdPulse AI · Real time crowd risk monitoring
*Mar 2026 – present · YOLOv8, OpenCV, PyTorch, Flask, SQLite, Next.js, Recharts · [Backend](https://github.com/Charan7sai/crowdpulse-backend), [Frontend](https://github.com/Charan7sai/crowdpulse-frontend)*

- YOLOv8 detection at 30 to 50 ms per frame behind a ~20 FPS live stream, with real time and historical data served over REST.
- Four level risk score from density, growth and persistence, stabilised with hysteresis and EMA smoothing to stop flicker between levels.
- Next.js dashboard with live detection overlay, density trend and heatmap, and graceful handling when the backend is offline.

### [LifeSignal AI](https://github.com/Charan7sai/LifeSignal-AI) · Life event engagement engine
*May 2026 · SBI Hackathon @ GFF 2026 · Scikit-learn, Pandas, LangChain*

- Random forest Life Stage Transition Index across 12 life event categories, reaching 79.9% test accuracy (79.4% 5 fold CV).
- A LangChain agent picks the best product once the index crosses a threshold and dispatches it over YONO, SMS or WhatsApp.

### [Loan Approval Prediction](https://github.com/Charan7sai/Loan_Prediction) · End to end classification pipeline
*Oct – Dec 2025 · Pandas, Scikit-learn, Joblib*

- Chose logistic regression over a decision tree (ROC-AUC 0.75 vs 0.66): 79% accuracy, F1 0.86 and recall 0.99 on unseen data.
- Validated features with a chi square test and a two sample t test, then saved a deployable pipeline.

### [Salary Prediction](https://github.com/Charan7sai/Salary_Prediction_EDA) · Linear regression on hiring data
*Jul – Sep 2025 · Pandas, Scikit-learn, Matplotlib, Seaborn*

- Predicts candidate CTC from real world hiring data with R² = 0.894 on the test set.
- EDA identified experience as the strongest salary predictor.

---

## Skills

### Programming
- **Languages:** Python, C, C++, Java, JavaScript, SQL, T-SQL, MATLAB

### Machine Learning
- **Classical ML:** Linear, Logistic & Ridge Regression, Decision Trees, Random Forest, LightGBM, DBSCAN Clustering, Scikit-learn
- **Deep Learning:** PyTorch, TensorFlow, Keras, RNN, LSTM, GRU, Encoder Decoder with Attention, Transformers (BERT), Transfer Learning
- **NLP & LLMs:** Hugging Face Transformers, Sentence-Transformers, Word2Vec, TF-IDF, Zero Shot Text Scoring, LangChain (Agents, Tool Routing), Vertex AI AutoML, Dialogflow, Entity Resolution, Fuzzy Matching (rapidfuzz)
- **Vision & Audio:** YOLOv8 (Ultralytics), OpenCV, MJPEG Streaming, CLAP Audio Text Embeddings, librosa, ffmpeg
- **Retrieval & Recommendation:** Cross Modal Retrieval, Cosine Similarity Search, Hubness Correction, Candidate Blocking, One to One Assignment Matching
- **Forecasting:** Walk Forward Backtesting, Quantile Regression, Conformal Prediction (CQR), LEAR / LASSO Autoregression, Lag & Calendar Features, Probabilistic Forecasting
- **Evaluation:** ROC-AUC, F1 / F0.5, Precision & Recall, K-Fold & GroupKFold CV, Threshold Optimisation, Ranking Metrics (Top-K, Percentile Rank), Benchmark Construction, Pinball Loss & Interval Coverage, Diebold–Mariano Test, SHAP Explainability

### Data
- **Analysis & Statistics:** Pandas, NumPy, SciPy, Matplotlib, Seaborn, Plotly, Chi Square & t Tests, EDA, Feature Engineering, Linear Programming (HiGHS)
- **Data Engineering:** Microsoft Fabric, Lakehouse & Warehouse, Data Factory Pipelines, Dataflows Gen2, Eventstreams & KQL, PySpark, Delta Lake, Parquet, SPARQL (Wikidata)
- **Databases:** SQLite, MongoDB (PyMongo), SQLAlchemy ORM, SQL, T-SQL
- **Cloud:** Google Cloud Vertex AI, Microsoft Fabric, Hugging Face Hub

### Web Development
- **Frontend:** HTML5, CSS, JavaScript, React, Next.js (App Router), Vue 3, Recharts, Chart.js, Streamlit, PWA
- **Backend:** FastAPI, Flask, Uvicorn, REST APIs, JWT Auth & RBAC, Redis Caching, Celery, Python Threading

### DevOps & Security
- **Tools & Platforms:** Git, GitHub, Docker, Docker Compose, GitHub Actions (CI/CD), pytest, Jupyter, Google Apps Script, AutoCAD
- **Security:** CI/CD Pipeline Attacks, Software Supply Chain Risk, IAM Misconfiguration, Credential Leakage, Container Security, Infrastructure as Code

---

## Education

| Degree | Institution | Details |
|---|---|---|
| B.Tech, Computer Science (AI/ML) | Manipal University Jaipur | GPA 8.08 / 10 · Expected 2028 |
| B.S., Data Science and Applications | IIT Madras (IITM BS programme) | Foundational level completed Dec 2025 · Pursuing alongside the B.Tech · Expected 2029 |

---

## Certifications

| Certification | Issuer | Date |
|---|---|---|
| Fabric Data Engineer Associate (DP-700) | Microsoft | Aug 2026 |
| Design & Analysis of Algorithms | NPTEL, IIT Madras | Mar 2026 |
| Industrial Training in Machine Learning | Intern Vision Technology (DPIIT Recognised) | Feb 2026 |
| Foundational Level, Programming & Data Science | IIT Madras | Dec 2025 |
| Natural Language Processing on Google Cloud | Coursera (Google Cloud) | Dec 2025 |
| Data Structures & Algorithms Design (Elite) | NPTEL, IIT Kanpur | Oct 2025 |

---

## Leadership & Activities

- **Student Placement Coordinator**, AI/ML department, Manipal University Jaipur *(Aug 2026 – present)*: placement coordinator for the entire department; share opportunities with students, run placement drives, and link students, the placement cell and recruiters.
- **Volunteer, Culturals Team**, IIT Madras *(Mar – Jun 2026)*: liaison between event teams and organisers at [Paradox ’26](https://paradox-showcase.web.app/).
- **Senior Event Coordinator**, IEEE Women in Engineering, MUJ *(Oct 2025 – May 2026)*: organised [Elysium 2.0](https://elysium-2-0-ten.vercel.app/), a multi day IEEE WIE fest with over Rs. 50,000 in prizes.
- **Senior Event Coordinator**, Teach For India, MUJ *(Sep 2025 – May 2026)*: hosted an awareness talk on rural education with three chief guests.

---

## Contact

- **Email:** [neelisettycharansai@gmail.com](mailto:neelisettycharansai@gmail.com)
- **GitHub:** [github.com/Charan7sai](https://github.com/Charan7sai)
- **LinkedIn:** [linkedin.com/in/charan-sai-neelisetty-616021328](https://www.linkedin.com/in/charan-sai-neelisetty-616021328/)
- **LeetCode:** [leetcode.com/u/Miles06](https://leetcode.com/u/Miles06/)

---

© 2026 Charan Sai Neelisetty
