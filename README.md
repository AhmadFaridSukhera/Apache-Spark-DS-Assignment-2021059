<h1>🎥 Netflix TV Shows & Movies Analysis with Spark & Scala</h1>
<p>This project performs exploratory data analysis (EDA) on the Netflix TV Shows and Movies dataset using Apache Spark and Scala.
</p>

<h1>📘 Table of Contents</h1>
<table>
<ul>Introduction</ul>
<ul>Key Spark Concepts</ul>
<ul>Setup Instructions</ul>
<ul>How to Run the Project</ul>
<ul>Results and Outputs</ul>
</table>

<h1>🚀 Introduction</h1>
<p>
Apache Spark is an open-source distributed computing system that provides an interface for programming entire clusters with implicit data parallelism and fault tolerance. It’s widely used for big data processing and supports multiple programming languages like Scala, Python, and Java.</p>

<h1>🔑 Key Spark Concepts</h1>
<h2>RDD - Core of Spark</h2>
Resilient Distributed Dataset (RDD) is Spark's core abstraction for a fault-tolerant and distributed collection of elements that can be operated on in parallel.

Execution in Spark
Spark employs a Directed Acyclic Graph (DAG) to plan jobs. It breaks operations into tasks and stages to optimize execution across distributed systems.

Memory Management
Spark uses a combination of in-memory processing and disk storage to optimize the use of resources and speed up data processing.

Fault Tolerance
Spark ensures fault tolerance by allowing RDDs to be rebuilt from lineage in case of node failures.

<h1>⚙️ Setup Instructions</h1>
Prerequisites
Install Docker on your machine.
Clone this repository:
git clone <repository-url>
cd <repository-folder>
🔧 How to Run the Project
1. Build the Docker Image
Build the Docker image for the Spark Scala application:

docker build -t spark-scala-app .
2. Run the Docker Container
Start a Docker container using the built image:

docker run --rm -v $(pwd)/output:/app/output spark-scala-app
4. View Output
The results will be saved in the output/ directory within the project directory


<h1>📊 Results and Outputs</h1>
Schema Information: Available in output/schema.txt.
Sample Data: First 10 records saved in output/sample_data/.
Movies vs. TV Shows Count: Results saved in output/type_count/.
Top 10 Countries with Most Titles: Results saved in output/top_countries/.
Popular Genres: Results saved in output/popular_genres/.
Titles Released Per Year: Results saved in output/titles_per_year/.
Null Counts: Null values for each column saved in output/null_counts.txt.


<h1>📖 Notes</h1>
Ensure that the path to the NetflixEDA.jar file is correctly specified in the Spark job submission command.
To map the output directory to your local machine, consider using Docker volumes or bindings.
