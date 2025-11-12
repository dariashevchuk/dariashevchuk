## Hi there 👋


I’m Dariia, the Artificial Intelligence student at Poznan University of Technology, semester 5/7. 
I am passionate about AI, ML and everything connected to it. 
Check out my recent projects:

## 1) Hate-2-Action
- About: a bot that reads user messages and suggests which projects or organizations may help the user to address their problems. It uses the sophisticated pipeline: user message is processed via RAG agent, it finds problems and solutions, then we create embeddings and use similarity vector search in order to match problems-solutions and solutions-projects, then we select top 3-5 best suitable projects and let the LLM write an reply. Works via CLI, API, Telegram bot, and a web app. The bot is implemented both in python and n8n. Such approach ensures the closest match of the response to the users needs.
- Research was done in order to compare the results of vector search (how to increase the value of cosine similarity between problems-solutions and then solution-projects) vs the length of the text for the LLM prompt (<300 chars, <800 chars or <1200 chars per problem/solution description). The optimum values of cos similarity appeared to be when the length of the output description per problem/solution is <800 chars.
- Tools used: Python, LangChain + OpenAI (LLM, embeddings), Scikit-learn, cosine similarity, SQLite/pgvector-ready, Next.js, react-markdown/remark-gfm, Docker Compose, Telegram Bot, Supabase Store, Postgres, Supabase vector store, Jupyter Notebook.  


## 2) Contribution for OpenPetitions (RAG for Ukrainian presidential petitions)

- About: The service that scrapes petitions from the Ukrainian president website. Analyzes petitions, groups topics, does semantic search, and shows trends. My contribution was based in the multi-label classification of the petitions. 
- Research was done. Comparison of Classification methods for OpenPetitions. How different embedding models, types of classification (llm-based, vector based, manual) influence the classification results, comparison of methods with the ground truth (manual classification of petitions).
- Tools used: Python, sentence-transformers / bge / OpenAI embeddings, cosine / dot / L2 / Manhattan / Hamming, notebooks, matplotlib, SQLite/Weaviate, Flask, basic dashboards.


## 3) Web-scraping Seed Agent
About: Scrapes sources and seeds a database with clean, structured data for later apps/bots.
Tools used: Python, Playwright/requests, JSON/CSV, SQLite/Supabase, Docker, simple ETL logic.


## 4) Movie-Explorer - React SPA with Concurrency Patterns
Tech: React 18, React Router, TMDb API, custom hooks, Python/JS, REST APIs, Flask/Next.js (depending on version), HTML/CSS.
What it is: Single-page app to search, inspect, and bookmark movies.
Concurrency aspects: Debounced search, concurrent fetch via useFetch, batched state updates, and localStorage sync via custom hooks.



## 5) Convex Optimization Project (group)
What it is: Graph optimization problem. Finds a minimal set of pairs (edges) such that every student is in at most one pair and remaining students form an independent set.
My part: Resourceful Students — Heuristic (RSH) 
Tech: C++ (simulated annealing + greedy / priority-queue algorithms)
What it is: Graph optimization problem. A fast solver for the same task with two regimes: Greedy initialization and simulated annealing with remove/swap moves under a 27s budget, and priority-queue by deg(u)+deg(v); picks edges with highest priority while keeping endpoints unmatched. 
Result: Submitted as dashashevchuk: Score 93.97, 774.55s.

## 6) FrogShopping — Graph Coverage with BFS
Tech: C++ (adjacency lists, BFS)
What it is: Place “shops” so every node is within distance D of at least one shop.
Approach: Greedy “pick & cover”: for each uncovered node, place a shop and BFS to radius D to mark coverage. O(N(N+M)) worst-case; much faster in practice. 98.22/100 points on Optil.io (submission dashashevchuk). 


## 7) OP — Airline Reservation System (group)
Tech: C++ (inheritance, polymorphism, file I/O), OOP/SOLID, UML, unit tests, Git.
What it is: Models airline ops: flights (domestic/international), passengers, reservations, payments, logging, and reports.
Design: Modular classes (Airline, Flight*, Passenger, Reservation, Payment, Report, Logger, Seat*), console UI, file-based persistence.


## 8) OP — Game Project (group)
Farm Simulation System
Tech: Java (threads, synchronization), OOP patterns, simple graphics/console UI, Git.
What it is: Multi-agent 2D farm where Farmer, Dog, Rabbit act in parallel; thread-safe Field/Tile grid; coordinated start/stop.
Learning: OOP + thread safety, shared state, and deterministic control over concurrent actors.


## 9) Deap Learning NN project 
Tech: NumPy, Pandas, TensorFlow, Keras,
What is it? We build a neural network that mimics the slow but exact function getProbability(df) for up to 16 validators.
Input per validator: two numbers — pActive ∈ [0,1] and popularity > 0.
Output: a probability for each validator that the nominator gets assigned to them. We also include one extra none option (no validator active) inside the model and drop it at the end.

## 10) Machine Learning Classifier Comparison (group)
Tech: EDA, PCA, one-hot encoding, scikit-learn, pandas, plotly, numpy, python
What is it? We take the Titanic dataset to perform EDA and later on compare K-NN, Logistic Regression, and Naive Bayes classifiers. 


## Molecular Counterfactuals 




