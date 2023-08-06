
> **Font:** Software Architecture Patterns - Mark Richards

# Definition

The space-based pattern (also called cloud architecture) is all about making applications really good at handling lots of work without slowing down. Instead of relying on one central database, it uses copies of data stored in memory across many computers. This makes it super fast and can handle a huge amount of work.

Imagine a website where people bid on items. In this pattern, the website can handle lots of bids happening at the same time because it doesn't rely on just one database. Instead, it spreads the work across many computers. This is like having a team of workers, each with their own copy of the important information. When a bid comes in, any available worker can update the info quickly and send it back to the website. This way, the website doesn't get overwhelmed even when lots of people are bidding at once.

This pattern operates on two major components:

## Virtualized Middleware

The virtualized-middleware is like the *manager of the system*. It takes care of important tasks like making sure data is up to date and handling requests. It has different parts like the messaging grid, data grid, processing grid, and deployment manager. These parts work together to make things run smoothly. They can be made by the team or bought from other companies.

## Processing Unit

The *processing unit* holds application logic, including web-based and backend components. It changes based on app size - small apps stay in one processing unit, whereas big apps split into multiple units. Each unit has app modules, in-memory data storage, and can save data for backup. It also has a replication engine for sharing data changes between units through the virtualized middleware.

![space_based_pattern](space_based_pattern.png)

## Conclusion

This pattern is one of the least used by companies, since it brings complexity to many layers of the application and make it the most difficult to develop on.