# NoSQL 

## Scenario and Its Understanding  

 Our project faces performance and scaling issues. So, my team lead asked me to check if a NoSQL database can help.
 - Performance issues is that When the system is slow and takes too much time to respond.
 - Scaling issues is that When the system fails or slows down if too many users uses it or huge data are added. 
 - For example: when a customer buys a pair of shoes online, the system needs to check data from many tables like Product table, Customer table, Address         table, Shipping table. For every request, the system must join those tables which takes more time and this will cause performance and scalling issues. 

---

## Why to use NoSQL and Not SQL ? 

- In Amazon when you check an order, the system has to join many tables like customer, product, payment, and shipping. 
- In SQL databases this requires a lot of joins and as the data grows, these joins become slower since SQL has a fixed structure.
NoSQL databases solve this problem because they can store all related data in one place (like one document). This means fewer joins are needed, and the system becomes faster.  
- SQL also depends on one big server (vertical scaling). So when millions of people uses it at the same time, it gets hard to share it. NoSQL can spread data 
across many servers, so it easily handles heavy traffic especially during an Amazon sale.  
- So, for performance and scaling issues, NoSQL (like MongoDB, Cassandra, Redis, Neo4j, CouchDB) is a better choice. 

---

## Types of NoSQL    

### 1. MongoDB  
   - MongoDB is a Document Database. It stores the data in JSON-like format. It is best for flexiblility and fast-changing data.  
   - Assume MongoDB as a notebook where each page has all the details about that one person.  
   - Realtime Example: Flipkart keeps our name, address, phone number, and order history on one page instead of splitting it into many tables.  
   - This makes it easy and fast to find our full details at one time.  

### 2. Cassandra  
   - Cassandra is a Wide-column store. It organizes data in rows and columns. unlike SQL tables, it can handle a huge amount of data spread across many server.  
   - Assume Cassandra as a giant library with many shelves spread across different cities but all working together.  
   - Realtime Example: Netflix uses it to store what movies we’ve watched. Imagine millions of people pressing play at the same time, Cassandra can handle this          because it spreads data across many servers.Even if one server fails the others still works, so the service doesn’t stop.  

### 3. Redis  
   - Redis is an In-Memory Key-Value Store, used for caching and real-time apps.  
   - It keeps data in memory (RAM) instead of on a hard disk.
   - Redis is like a whiteboard in a classroom, we can write and erase things very fast.  
   - Realtime Example: In online games, Redis stores live scores and rankings and you can instantly see who’s winning.  

### 4. CouchDB  
   - CouchDB is a Document-oriented. It stores data as JSON and syncs easily across devices which makes it easy to share and update data.  
   - Assume CouchDB as a notebook that automatically copies itself into your phone, laptop, or tablet.  
   - Realtime Example: In apps like Evernote, when you type a note on your laptop, it shows up on your phone too. CouchDB handles this syncing of data across            devices.    

### 5. Neo4j  
   - Neo4j is a Graph database. It is best for social networks, recommendations, where data is connected like a web.  
   - Neo4j stores data as (Nodes represent entities like people, products), Relationships (represent how those entities are connected like friend of, bought),
     Properties (extra information attached to nodes or relationships like age, date, product price).
   - Example: On LinkedIn when you connect with someone, Neo4j helps the system show “People You May Know” because it knows how you and others are linked.

## References 

- https://youtu.be/kOZehgi8vPk?si=kC-JRpaFdpouOxmR
  
- https://youtu.be/kkeFE6iRfMM?si=vua_uhhtrkx1-I56

- https://youtu.be/0buKQHokLK8?si=isHRDA6r75SMOzwa

- https://share.google/ruDZ4Rrmidi0Ocft8

- https://share.google/yBqkGBks8caqAk7W9
  
- www.google.com

