
### SpringBoot API + SpringSecurity ###
#### Group: André  Madruga Paulo, Nikolay Novachuk, Dominique Tavares Ganime Bastos####

*API to test the knowledge acquired during the bootcamp.*

Name of the project: **Backend-to-Frontend-Services**


This project aims to simulate a simple online shopping list for a user, where he aims to create his personal data using his personnal password and name, and edit it. Also, each created user is able to pick up different grocery products and create new invoce, knowing the total price of each invoice, consult his personal invoices, navigate the data added to database.

This API consists of 4 models, of whom 3 are classes and 1 extenda a package of the SpringSecurity configuration:

* Models:
  * Classes
    * Invoice
    * Product
    * User                                                              
   * SecurityConfiguration:
    * UserDetails
    
To define a better method of storing, updating, and extracting the data stored from JAVA applications in the backend we use 3 repositories for our application purpose
* Repositories
  * InvoiceRepository
  * ProductRepository
  * UserRepository
  
With a specific functionality "service" we will check whether the given data is valid or not, using our Requests and Resposes, created for 3 main classes.
* Services
  * InvoiceService
  * ProductService
  * US 
    * UserService - is used for a purpose of the SpringSecurity configuration

To invoke business logic update the model and returns the view that should be rendered we use controllers which are responsible for processing incoming requests.
* Controllers
  * InvoiceController
  * ProductController
  * UserController
  
 * Endpoints:
    * Post: 
      * **NewProduct** - creates a product
      * **NewInvoice** - add products and associate an invoice to the user
    * Get:
      * **GetAllInvoices** - retrieves the invoices of a user
      * **GetInvoiceByName** - retrieves an invoce by it's name
      * **GetAllProducts** - retrieve all products
      * **FindInvoicesById** - retrieve a product by its id    
    * Put:
      * **User** - modifies the User info
      
 * Exceptions
   * ResourceNotFound
     * Invoice Not Found
     * Add a valid name to invoice
