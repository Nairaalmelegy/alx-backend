# 0x03. Queuing System in JS


## Tasks
0. Redis installation and setting the value `School` for the key `Holberton`
1. Script that connects to redis servers running locally

2. Functions:
    - `SetNewSchool` - sets value for given key
    - `displaySchoolValues` - retrieves value of given key

3. Extension of 1-redis_op.js that modifies `displaySchoolValue` function to work using promises.

4. Script that sets redis hashes using `node-redis` and prints the response using `redis.print`
5. Pub-Sub model in redis:
    - Script that creates a redis client and subscribes it to `holberton school channel`
    - Scripts that creates a redis client that published to `holberton school channel`
6. Job creation using `kue`

7. Job processing using `kue`

8. Tracking job progress and errors with `kue` - **job creator**

9. Tracking job progress and errors with `kue` - **job processor**

10. Job creation function `createPushNotificationsJobs`

11. Unit tests for `createPushNotificationsJobs`

12. Express orders API server that uses redis for caching:
    - Routes:
        - `GET /list_products/`: returns a list of all products.
        - `GET /list_products/:itemId`: returns information about products with specified id.
        - `GET /list/reserve_product/:itemId`: reservers one unit of product with given item id if present and in stock.

13. Express seat reservation API server that uses redis for job queues:
    - Routes:
        - `GET /available_seats`: returns the number of available seats.
        - `GET /reserve_seat`: seat reservation endpoint.
        - `GET /process`: reservation jobs processing endpoint.
