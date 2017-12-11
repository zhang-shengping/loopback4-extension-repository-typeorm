# Feature comparison between LoopBack and TypeORM

## Major features

| Feature                 | TypeORM                                                                                  | LoopBack                                                                                                                                                                                                                                                                                                                          |
| ----------------------- | ---------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Databases               | MySQL<br>PostgreSQL<br>MariaDB<br>SQLite<br>MS SQL Server<br>MongoDB<br>Oracle<br>WebSQL | In-memory<br>MySQL<br>PostgreSQL<br>SQLite<br>MS SQL Server<br>Oracle<br>MongoDB<br>Cloudant<br>CouchDB<br>DB2<br>DB2 Z<br>DB2 iSeries<br>DashDB<br>Informix<br>Cassandra<br>Key Value (...)<br><hr>ElasticSearch<br>https://github.com/pasindud/awesome-loopback<br>https://www.npmjs.com/search?q=loopback-connector (189 hits) |
| Model Definition        | TypeScript classes with decorators                                                       | JSON<br>TypeScript classes with decorators                                                                                                                                                                                                                                                                                        |
| Data access patterns    | ActiveRecord (BaseEntity)<br>EntityManager<br>Repository                                 | ActiveRecord (3.x Model)<br>Repository (4.x)                                                                                                                                                                                                                                                                                      |
| Database Adapters       | QueryRunner (monorepo)                                                                   | Connector (multiple repos/modules)                                                                                                                                                                                                                                                                                                |
| Query                   | QueryBuilder                                                                             | Filter JSON Object<br>FilterBuilder (4.x)                                                                                                                                                                                                                                                                                         |
| Scopes                  | No                                                                                       | Yes                                                                                                                                                                                                                                                                                                                               |
| Mutation                | QueryBuilder                                                                             | Where JSON Object                                                                                                                                                                                                                                                                                                                 |
| Feedback from mutations | No                                                                                       | Yes                                                                                                                                                                                                                                                                                                                               |
| Mixins                  | No                                                                                       | Yes                                                                                                                                                                                                                                                                                                                               |
| Transaction             | Yes                                                                                      | Yes                                                                                                                                                                                                                                                                                                                               |
| Optimistic Locking      | Yes                                                                                      | No (requested by AppConnect team)                                                                                                                                                                                                                                                                                                 |
| Connection pooling      | Yes                                                                                      | Yes                                                                                                                                                                                                                                                                                                                               |
| Relations               | Yes                                                                                      | Yes                                                                                                                                                                                                                                                                                                                               |
| Relational Join         | Yes                                                                                      | No                                                                                                                                                                                                                                                                                                                                |
| Discovery               | No                                                                                       | Yes                                                                                                                                                                                                                                                                                                                               |
| Migration               | Yes                                                                                      | Yes                                                                                                                                                                                                                                                                                                                               |

## Side by side claims by TypeORM

| Claimed by TypeORM                                               | LoopBack                                                             |
| ---------------------------------------------------------------- | -------------------------------------------------------------------- |
| supports both DataMapper and ActiveRecord (your choice)          | DataMapper is supported by Repository and ActiveRecord by 3.x models |
| entities and columns                                             | Yes                                                                  |
| database-specific column types                                   | Yes                                                                  |
| entity manager                                                   | Connectors                                                           |
| repositories and custom repositories                             | Yes                                                                  |
| clean object relational model                                    | Yes                                                                  |
| associations (relations)                                         | Yes                                                                  |
| eager and lazy relations                                         | Yes                                                                  |
| uni-directional, bi-directional and self-referenced relations    | Yes                                                                  |
| supports multiple inheritance patterns                           | Polymorphic relations                                                |
| cascades                                                         | No                                                                   |
| indices                                                          | Yes                                                                  |
| transactions                                                     | Yes                                                                  |
| migrations and automatic migrations generation                   | Yes                                                                  |
| connection pooling                                               | Yes                                                                  |
| replication                                                      | Depending on the driver                                              |
| using multiple database connections                              | Yes                                                                  |
| working with multiple databases types                            | Yes                                                                  |
| cross-database and cross-schema queries                          | Yes                                                                  |
| elegant-syntax, flexible and powerful QueryBuilder               | Poc in 4                                                             |
| left and inner joins                                             | No                                                                   |
| proper pagination for queries using joins                        | No                                                                   |
| query caching                                                    | No                                                                   |
| streaming raw results                                            | No                                                                   |
| logging                                                          | Yes - debug                                                          |
| listeners and subscribers (hooks)                                | Yes                                                                  |
| supports closure table pattern                                   | No                                                                   |
| schema declaration in models or separate configuration files     | Yes                                                                  |
| connection configuration in json / xml / yml / env formats       | Yes                                                                  |
| works in NodeJS / Browser / Ionic / Cordova / Electron platforms | NodeJS only, 3.x is compatible with Browser                          |
| TypeScript and JavaScript support                                | Yes                                                                  |
| produced code is performant, flexible, clean and maintainable    | ?                                                                    |
| follows all possible best practices                              | ?                                                                    |
| CLI                                                              | Yes                                                                  |