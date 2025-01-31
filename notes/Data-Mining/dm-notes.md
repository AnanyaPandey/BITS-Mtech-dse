
### What is Data Mining 
Data Mining is knowledge discovery from the data. Extraction of interesting (non-trivial, implicit, previously unknown and potentially useful) patterns or knowledge from huge amount of data Knowledge discovery (mining) in databases (KDD), knowledge extraction, data/pattern analysis, data archaeology, data dredging, information harvesting, business intelligence, etc.

### Why Data Mining ?

* The Explosive Growth of Data: from petabytes to zetabytes
* Data collection and data availability - Automated data collection tools, database systems, Web, computerized society
* Major sources of abundant data
    * Business: Web, e-commerce, transactions, stocks,
    * Science: Remote sensing, bioinformatics, scientific simulation,
    * Society and everyone: news, digital cameras, YouTube 
    

Data Mining in business Intelligence :
![](images\dm1.jpg)

Data Mining or Knowledge discovery process. 
![](images\dm2.jpg)

There are different types of data on which mining can be performed. Besides relational database data (from operational or analytical systems), there are many other kinds of data that have diverse forms and structures and different semantic meanings

* time-related or sequence data (e.g., historical records, stock exchange data, and time-series and biological sequence data), 
* data streams (e.g., video surveillance and sensor data, which are continuously transmitted), 
* spatial data (e.g., maps), 
* engineering design data (e.g., the design of buildings, system components, or integrated circuits), 
* hypertext and multimedia data (including text, image, video, and audio data), 
* graph and networked data (e.g., social and information networks), and 
* the Web (a widely distributed information repository). 

## Data Mining Tasks :

* Description - Find human-interpretable patterns that describe the data
    * Clustering [Descriptive]
    * Association Rule Discovery [Descriptive]
    * Sequential Pattern Discovery [Descriptive]

* Prediction - Use some variables to predict unknown or future values of other variables.
    * Classification [Predictive]
    * Regression [Predictive]
    * Deviation Detection [Predictive]

### DM Process and challenges
The standard data mining process involves. A popular data mining process frameworks is CRISP-DM (Cross Industry Standard Process for Data Mining). 

* understanding the problem, 
* preparing the data (samples), 
* developing the model, 
* applying the model on a data set to see how the model may work in real world, and 
* production deployment

### Generic Data Mining Process.
![](images\dm3.jpg)

### Prior Knowledge
Can be different for each person or organization. 

### Data Preparation
Data needs to be understood. Basic Data exploration requires descriptive statistics such as mean, median, mode, standard deviation, and range for each attribute. Data quality is an ongoing concern wherever data is collected, processed, and stored. 

    * The data cleansing practices include elimination of duplicate records, quarantining outlier records that exceed the bounds, standardization of attribute values, substitution of missing values, etc.
    * it is critical to check the data using data exploration techniques in addition to using prior knowledge of the data and business before building models to ensure a certain degree of data quality
    * Missing Values - Need to track the data lineage of the data source to find right solution
    * Data Type and Conversion - The attributes in a data set can be of different types, such as continuous numeric (interest rate), integer numeric (credit score), or categorical
    * Transformation - Can go beyond type conversion, may include dimensionality reduction or numerosity reduction
    * Outlier - Outlier detection, treatment and outlier handling.
    * Feature Selection - Many data mining problems involve a data set with hundreds to thousands of attributes, most of which may not be helpful. Some attributes may be correlated, e.g. sales amount and tax
    
### Modeling and Evaluation
A model is the abstract representation of the data and its relationships in a given data set.
Data mining models can be classified into the following categories: classification, regression, association analysis, clustering, and outlier or anomaly detection. Each category has a few dozen different algorithms; each takes a slightly different approach to solve the problem at hand

### DM Issues and Challenges

#### Mining Methodology
Mining Methodology involves the investigation of new kinds  of knowledge, mining in multidimensional space, integrating methods from other disciplines, and the consideration of semantic ties among data objects. 

* **Mining various and new kinds of knowledge**: Data mining covers a wide spectrum of data analysis and knowledge discovery tasks, from data characterization and discrimination to association and correlation analysis, classification, regression, clustering, outlier analysis, sequence analysis, and trend and evolution analysis. 
* **Mining knowledge in multidimensional space**: When searching for knowledge in large data sets, we can explore the data in multidimensional space. That is, we can search for interesting patterns among combinations of dimensions (attributes) at varying levels of abstraction. Data can be aggregated or viewed as a multidimensional data cube. 
* **Data mining—an interdisciplinary effort**: For example, to mine data with natural language text, it makes sense to fuse data mining methods with methods of information retrieval and natural language processing, e.g. consider the mining of software bugs in large programs, known as bug mining, benefits from the incorporation of software engineering knowledge into the data mining process.
* **Boosting the power of discovery in a networked environment**: Most data objects reside in a linked or interconnected environment, whether it be the Web, database relations, files, or documents. Semantic links across multiple data objects can be used to advantage in data mining.
* **Handling uncertainty, noise, or incompleteness of data**: Data often contain noise, errors, exceptions, or uncertainty, or are incomplete. Errors and noise may confuse the data mining process, leading to the derivation of erroneous patterns. Data cleaning, data preprocessing, outlier detection and removal, and uncertainty reasoning are examples of techniques that need to be integrated with the data mining process.
* **Pattern evaluation and pattern- or constraint-guided mining**: What makes a pattern interesting may vary from user to user. Therefore, techniques are needed to assess the interestingness of discovered patterns based on subjective measures. These estimate the value of patterns with respect to a given user class, based on user beliefs or expectations. 


#### User Interaction
The user plays an important role in the data mining process. Interesting areas include how to interact with a data mining system, how to incorporate a user's background knowledge in mining, and how to visualize and comprehend data mining results. 

* **Interactive mining:** The data mining process should be highly interactive. Thus, it is important to build flexible user interfaces and an exploratory mining environment, facilitating the user's interaction with the system. A user may like to first sample a set of data, explore general characteristics of the data, and estimate potential mining results. Interactive mining should allow users to dynamically change the focus of a search, to refine mining requests based on returned results, and to drill, dice, and pivot through the data and knowledge space interactively, dynamically exploring "cube space" while mining.
* **Incorporation of background knowledge**: Background knowledge, constraints, rules, and other information regarding the domain under study should be incorporated into the knowledge discovery process. Such knowledge can be used for pattern evaluation as well as to guide the search toward interesting patterns.
* **Ad hoc data mining and data mining query languages**: Query languages (e.g., SQL) have played an important role in flexible searching because they allow users to pose ad hoc queries. Similarly, high-level data mining query languages or other high-level flexible user interfaces will give users the freedom to define ad hoc data mining tasks. This should facilitate specification of the relevant sets of data for analysis, the domain knowledge, the kinds of knowledge to be mined, and the conditions and constraints to be enforced on the discovered patterns. Optimization of the processing of such flexible mining requests is another promising area of study.
* **Presentation and visualization of data mining results:** How can a data mining system present data mining results, vividly and flexibly, so that the discovered knowledge can be easily understood and directly usable by humans? This is especially crucial if the data mining process is interactive. It requires the system to adopt expressive knowledge representations, user-friendly interfaces, and visualization techniques.


#### Efficiency and Scalability
Efficiency and scalability are always considered when comparing data mining algorithms. As data amounts continue to multiply, these two factors are especially critical.

* **Efficiency and scalability of data mining algorithms**: Data mining algorithms must be efficient and scalable in order to effectively extract information from huge amounts of data in many data repositories or in dynamic data streams. In other words, the running time of a data mining algorithm must be predictable, short, and acceptable by applications. Efficiency, scalability, performance, optimization, and the ability to execute in real time are key criteria that drive the development of many new data mining algorithms.
* **Parallel, distributed, and incremental mining algorithms:** The humongous size of many data sets, the wide distribution of data, and the computational complexity of some data mining methods are factors that motivate the development of parallel and distributed data-intensive mining algorithms. Such algorithms first partition the data into "pieces." Each piece is processed, in parallel, by searching for patterns. The parallel processes may interact with one another. The patterns from each partition are eventually merged.
* **Cloud computing and cluster computing**, which use computers in a distributed and collaborative way to tackle very large-scale computational tasks, are also active research themes in parallel data mining. In addition, the high cost of some data mining processes and the incremental nature of input promote incremental data mining, which incorporates new data updates without having to mine the entire data "from scratch." Such methods perform knowledge modification incrementally to amend and strengthen what was previously discovered.


#### Diversity of Database Types
* **Handling complex types of data:** Diverse applications generate a wide spectrum of new data types, from structured data such as relational and data warehouse data to semi-structured and unstructured data; from stable data repositories to dynamic data streams; from simple data objects to temporal data, biological sequences, sensor data, spatial data, hypertext data, multimedia data, software program code, Web data, and social network data. It is unrealistic to expect one data mining system to mine all kinds of data, given the diversity of data types and the different goals of data mining. Domain- or application-dedicated data mining systems are being constructed for in-depth mining of specific kinds of data. The construction of effective and efficient data mining tools for diverse applications remains a challenging area.
* **Mining dynamic, networked, and global data repositories**: Multiple sources of data are connected by the Internet and various kinds of networks, forming gigantic, distributed, and heterogeneous global information systems and networks. The discovery of knowledge from different sources of structured, semi-structured, or unstructured yet interconnected data with diverse data semantics poses great challenges to data mining. Mining such gigantic, interconnected information networks may help disclose many more patterns and knowledge in heterogeneous data sets than can be discovered from a small set of isolated data repositories. Web mining, multisource data mining, and information network mining have become challenging and fast-evolving data mining fields.


#### Society
How does data mining impact society? What steps can data mining take to preserve the privacy of individuals? Do we use data mining in our daily lives without even knowing that we do? 

* **Social impacts of data mining:** With data mining penetrating our everyday lives, it is important to study the impact of data mining on society. How can we use data mining technology to benefit society? How can we guard against its misuse? The improper disclosure or use of data and the potential violation of individual privacy and data protection rights are areas of concern that need to be addressed.
* **Privacy-preserving data mining:** Data mining will help scientific discovery, business management, economy recovery, and security protection (e.g., the real-time discovery of intruders and cyberattacks). However, it poses the risk of disclosing an individual's personal information. Studies on privacy-preserving data publishing and data mining are ongoing. The philosophy is to observe data sensitivity and preserve people's privacy while performing successful data mining.
* **Invisible data mining:** We cannot expect everyone in society to learn and master data mining techniques. More and more systems should have data mining functions built within so that people can perform data mining or use data mining results simply by mouse clicking, without any knowledge of data mining algorithms. Intelligent search engines and Internet-based stores perform such invisible data mining by incorporating data mining into their components to improve their functionality and performance. This is done often unbeknownst to the user. For example, when purchasing items online, users may be unaware that the store is likely collecting data on the buying patterns of its customers, which may be used to recommend other items for purchase in the future.

## Data Pre-processing
* To improve data quality
* To modify data to better fit specific data mining technique

#### Major Tasks in Data Preprocessing
* Data cleaning
    * Fill in missing values, smooth noisy data, identify or remove outliers, and resolve inconsistencies
* Data integration
    * Integration of multiple databases, data cubes, or files
* Data reduction
    * Dimensionality reduction
    * Numerosity reduction
    * Data compression
* Data transformation and data discretization
    * Normalization 
    * Concept hierarchy generation

#### Data Quality ?
* What kinds of data quality problems?
* How can we detect problems with the data? 
* What can we do about these problems? 
* Examples of data quality problems: 
    * Noise and outliers 
    * missing values 
    * duplicate data 


### Data Clearning 
Data in the Real World Is Dirty: Lots of potentially incorrect data, e.g., instrument faulty, human or computer error, transmission error

* incomplete: lacking attribute values, lacking certain attributes of interest, or containing only aggregate data
    * e.g., Occupation = “ ” (missing data)
* noisy: containing noise, errors, or outliers
    * e.g., Salary = “−10” (an error)
* inconsistent: containing discrepancies in codes or names, e.g.,
    * Age = “42”, Birthday = “03/07/2010”
    * Was rating “1, 2, 3”, now rating “A, B, C”
    * discrepancy between duplicate records

#### Incomplete (Missing) data
* Data is not always available
E.g., many tuples have no recorded value for several attributes, such as customer income in sales data
* Missing data may be due to 
    * equipment malfunction
    * inconsistent with other recorded data and thus deleted
    * Relevant data not entered due to misunderstanding
    * certain data may not be considered important at the time of entry
* Missing data may need to be inferred

#### How to handle missing data
* Ignore the tuple: usually done when class label is missing (when doing classification)—not effective when the % of missing values per attribute varies considerably
* Fill in the missing value manually: tedious + infeasible?
* Fill in it automatically with 
    * a global constant : e.g., “unknown”, a new class?! 
    * the attribute mean
    * the attribute mean for all samples belonging to the same class: smarter
    * the most probable value: inference-based such as *Bayesian formula or decision tree*
    
 

```markdown
SKIPPED THESE 

Noise
Outliers
* Data integration
    * Integration of multiple databases, data cubes, or files
* Data reduction
    * Dimensionality reduction
    * Numerosity reduction
    * Data compression
* Data Transformation
    * Discretization
```

#### Normalization :
Bringing the features to same scale is called normalization. 

* Transforming the data to fall within a smaller or common range such as [-1, 1] or [0.0, 1.0]
* Normalising the data attempts to give all attributes an equal weight
* It also helps preventing attributes with larger values from outweighing attributes with smaller values.

##### Various methods
* Min-max normalization
* Decimal scaling
* Z-score

#### Min-max normalization: to [new_minA, new_maxA]

$$ v = \frac{v - min_A}{max_A - min_A} $$

