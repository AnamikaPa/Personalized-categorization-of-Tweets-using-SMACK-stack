# Personalized-categorization-of-Tweets-using-SMACK-stack
<ul>
  <li>Applied Real-time analytics which includes ingestion, processing, transformation, and analyzes of data at real-time speed.
  <li>Made use of SMACK (Spark, Mesos, Akka, Cassandra, Kafka) in order to brings together key open source technologies that work together to accelerate the data pipeline from processing to analysis, also make system fault tolerant and resilient.
  <li>A Dash board that can be accessed by logging into Twitter and it contains Personalized and Popular Sports News which is sorted and categorized into different sports by using Machine Learning Algorithms.
  <li><b>Skills:</b> Scala, Python, Real-Time Data, Natural Language Processing and Machine Learning
  <li><b>Note:</b> The project was a part of Wipro internship and according to their policies we are not allowed to share the code.
</ul>

<h2>Breif Project Flow: </h2>
<ul> 
  <li> Fetching real time data from Twitter Streaming API with tracks like espn, starsport, tensports, etc.
      <ul>
        <li>Getting Twitter API Keys.
        <li>Connecting to Twitter Streaming API and Downloading Data.
      </ul>
  <li> Fetching of Twitter data is done via <b>Akka</b> Http service to ensure concurrent, distributed and resilient message driven application.
  <li> Prepared a Dashboard using PHP, Spring boot, HTML, CSS, Javascript and AJAX.
  <li> Dash board is accessible after twitter login which provides the back-end with User's twitter ID. 
  <li> Using User ID we fetch the information like user's followings, likes/dislikes, retweet topics etc. We then filter this to contain only sports related information.  
  <li> Real time twitter data is then transferred to <b>Apache Kafka</b>, which served as a message buffer queue. 
  <li> Key Features of Kafka includes:
    <ul>
      <li> Handling the abnormalities in real time data feeds.
      <li> Ensuring Low latency which means it process very high volume of data messages with minimal delay(latency). 
      <li> Distribute and Partition the data among its Clusters.
      <li> Guarantee for Fault-Tolerance.
    </ul>
  <li> Kafka sends message to <b>Apache Spark</b> which is based on Hadoop MapReduce and it extends the MapReduce model to efficiently use it for more types of computations, which includes interactive queries and stream processing.
  <li> Key Features of Spark includes: 
    <ul>
      <li> High data processing speed of about 100x faster in memory and 10x faster on disk. 
      <li> Provides Fault tolerance through Spark Resilient Distributed Data set(RDD).
      <li> Real time data stream processing using Spark Streaming. 
      <li> Provide support for Sophisticated Analysis as it comes with dedicated tools which add on to map and reduce. 
    </ul>
   <li> Data Analytics steps in Spark includes:
     <ul>
       <li> Cleaning the data using Natural Language Processing like tokenization, stop word removal, slang correction etc. 
       <li> Extracting features using Bag of words, Part of Speech tagging, etc.
       <li> Converting unstructured data into structured format. 
       <li> Applying Machine learning algorithms to categorize tweets into different sports. 
     </ul>
  <li> Outcome of Data Analytics is stored in <b>Apache Cassandra</b> which is known for managing large amount of structured data across multiple servers. 
  <li> Key Features of Cassandra includes: 
      <ul>
        <li> High Scalability.
        <li> Fault Tolerance as multiple nodes in a cluster have a copy of same data.
        <li> High Availability.
      </ul>
    <li> All the components including Akka, Kafka, Spark and Cassandra is transferred on <b>Apache Mesos</b> which is an open source cluster manager.
    <li> Key Features of Mesos includes: 
      <ul>
        <li>Efficient CPU and memory aware resource scheduling among other SMACK stack components.
        <li> Ensures Scalability.
        <li> High Availability.
      </ul>
    <li> The Categorized tweets outcome is shown on UI which is modified according to user's preferences.
</ul>
