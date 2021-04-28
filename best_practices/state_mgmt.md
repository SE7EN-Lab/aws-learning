- Storing state locally in an instance/application is an anti-pattern as the state will be lost if the instance/app goes through scaling event.
- Share state with instance/application using in-memory object caching systems like Redis. Doing so, any new instance of the backend application starting will be able to get the previous state of the application from the cache and get on with the tasks at hand.
- Do not store transient state in (SQL) databases, use specialised datastore for that. Got some lists, sets, sorted sets, hashes or keys that store transient state? use Redis (for example) since it was built for that very purpose.

- If you are going to store something in your (SQL) database, make sure it is data that won’t be mutated shortly after, otherwise, it is a waste of database scalability credits.
Redis,DynamoDB, Memcached or Elasticsearch are great tools that can help take the load off your SQL databases, especially when you start scaling.

