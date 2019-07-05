## Web server log analysis and anomaly detection

### Details
There is a Kafka topic which has Nginx web server logs. Write an application to consume these logs, and - 
- Produce daily statistics, like number of valid requests, number of invalid requests, unique visitors, referrers, 404s, user-agents, hosts etc. 
- Group these statistics by referrers, hosts etc.
- Calculate daily bandwidth consumption
- Analyse/Detect different web attacks, like SQL Injection, DoS attack etc. 

When the date rotates, this application should dump previous day’s data in the filesystem in a consumable (like csv) format. 

Application should run through command line and must be designed to support scalability and fault tolerance. Please include proper tests and documentation. Also provide necessary Dockerfile and Docker compose configurations for build and test. 

Keep it simple. Focus on data. We would like to see your programming skills, so focus on good programming practices, design and data structures. 

You can use Python, Golang, Java, Rust or Scala. Please do NOT use any big-data frameworks like Spark, Flink etc. 

### Deliverables
Write proper tests and documentation. Deliver your source code in a public Github repo. Include Dockerfile and Docker compose configurations (if required) for build and test. 

### Logs
You can download sample logs from this repo. You can play these logs into your Kafka topic to generate your test dataset.

### References 
- https://goaccess.io/
- https://code.google.com/archive/p/apache-scalp/
- https://docs.nginx.com/nginx/admin-guide/monitoring/logging/
- https://hub.docker.com/r/bitnami/kafka/
- https://www.webopedia.com/TERM/D/DoS_attack.html






