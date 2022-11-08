# SpringNotes

Components: Controller, Service, and Repository

Controller is annotated with @RestController, handles incoming requests and building the response. 

Service is annotated with @Service, contains all business logic, describes verbs/actions, ensures business object state. Often has the same methods of repository but with a different focus. 

Repository is annotated with @Repository, describes nouns of the system. One to one object mapping

@Service - specifies you intend to use the class as part of your service layer
@Repository - marks a class as part of your data layer, for handling storage, retrieval, and search
@RestController - Component: combines the @Controller and @ResponseBody into a single annotation


@Autowired - Autowiring is the process of placing an instance of one bean into the specified field in an instance of another bean
@Entity - used to mark the persistence objects stores as records in the database

@OneToMany - used to define a one to many relationship between an object and alist of objects one-to-many mapping means that one row in a table is mapped to multiple rows in another table. Ex: One cart can have many items.
@ManyToOne -  where one entitiy contains values that refer to another entitiy. allows for a bidrectional relationship: we are able to access x from y AND also y from x

@Id -  specifies the primary key of an entity
@JoinColumn - helps us specify the column we'll use for joining an entity association or element collection
@Column - used to specify the mapped column for a persistent property or field
@GeneratedValue - provides for the specification of generation strategies for the values of primary keys
@Bean - useful if you have a class that requires an instance of another class as a property
@RequestParam -  allows you to send parameters in the get request and use them in Java

Spring Boot works with apps by using build and dependencies. Maven is a tool that is used to specify what dependencies or libraries the application will use for compiling and packaging for development. 

Spring boot works with spring applications by Using build and dependency managment. 
Maven and Gradle are build tools ised to specify what dependencies or libraries the application will use for compilation and packaging for deployment.
Project Layout and structure is partly tied to a maven project layout mixed with spring annotations to help identify different architectural pieces of the application. 

Spring boot Starters are packages or wrappers onto spring popular frameworks like spring MVC, Spring data, Spring Batch etc.. When adding a dependency like spring boot MVC the spring boot MVC starter will integrate and setup that library so it is fully configured and ready to use. Embeded Servers Apache Tomcat, Jetty-Undertow




