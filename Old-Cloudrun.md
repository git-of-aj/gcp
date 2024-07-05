## Requirements
Cloud run
As the  use cases are mostly *stateless, https and event based or batch jobs*, Cloud run will be used that helps to **containerize the applications and deploy to cloud**. Both cloud run services and cloud run job will be used.

●	Cloud run Services: Cloud run services will be used to create stateless, `https java-based services that can be invoked from the front-end applications like creating an item, ingesting an item or managing an item`. It can also be used to create micro-frontend applications for example in item management item creation and editing can be a micro-frontend application and handling of item can be another micro-frontend.
 
●	Cloud run jobs: In our application, `regular updates to the item catalog will be done by running batch jobs that incorporate new items, remove discontinued items, and update item` details. This will be a cloud run job.
 
3.2.2	Google Pub Sub
Pub/Sub will be used  applications for distributed transactions, real time event distribution and as an enterprise event bus and other use cases as needed. When `item prices change, the pricing system publishes an "ItemPricingUpdated" event to the pub/sub topic`
 
3.2.3	Database
Cloud SQL is the database chosen.
 
3.2.4	Memory store
Google Cloud MemoryStore this will be cached in redis memory store.
 
3.2.5	Cloud storage
Google Cloud Storage is an object storage service provided by Google Cloud Platform (GCP) that allows you to store and retrieve data in a scalable, durable, and highly available manner. Cloud Storage is designed for a wide range of use cases, `from storing and serving static assets for web applications to handling large-scale data analytics.`
 
3.2.6	Cloud functions
Google Cloud Functions is a serverless compute service provided by Google Cloud Platform (GCP) that allows you to run code in response to various events without the need to manage servers or infrastructure. In our Application, `cloud functions can be used to trigger notifications or alerts to relevant stakeholders when specific item-related events occur, such as low stock levels or critical updates.`
 
3.2.7	Google Operation Suite
It provides a set of tools and services designed to help monitor, troubleshoot, the  applications and services running on Google Cloud Platform (GCP) as well as on-premises and multi-cloud environments. It offers various features for monitoring, logging, profiling and tracing.
