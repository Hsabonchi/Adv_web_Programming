#Java #Hibernate # Maven. # SpringBoot
---
* [JPA-Tutorial](https://github.com/RameshMF/JPA-Tutorial)
* [Interface EntityTransaction](https://www.objectdb.com/api/java/jpa/EntityTransaction).
* [Hibernate Query Language](https://www.tutorialspoint.com/hibernate/hibernate_query_language.htm)
---
*`@ElementCollection` is mainly for mapping non-entities.
   * It means that the collection is not a collection of entities, but a collection of simple types (Strings, etc.) or a collection of  embeddable elements 
* `@OneToMany` is used to map entities
* .getSingleResult()
   * Execute a SELECT query that returns a single result.
   *  Specified by: getSingleResult() in Query
   *   Returns:
   *   the result
   *  Throws:
   * NoResultException - if there is no result.
* JPA  Operations that modify database content, such as a store, update, and delete should only be performed within an active transaction.
  	---
  - `entityManager.getTransaction().begin();`
  - `entityManager.getTransaction().commit();`
  - `entityManagerFactory.close();`
   


---
Common Errors
---
 * hibernate_sequence  does not exist. 
    * [error performing isolated work](https://coderanch.com/t/487173/databases/hibernate-sequence-exist).
 * PK mappmed to FK [@JoinColumn](https://stackoverflow.com/questions/11938253/whats-the-difference-between-joincolumn-and-mappedby-when-using-a-jpa-onetoma)
