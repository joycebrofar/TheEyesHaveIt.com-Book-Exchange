# 1. Use Case Descriptions
Use Case 1: Add Seller
- Use Case Name: Add Seller
- Actors: Seller, System
- Preconditions:
    - The seller must have a valid email address.
    - The seller must be registered on TheEyesHaveIt.com.
- Postconditions:
    - The seller's information is stored in the system.
    - The seller has an open account.
- Main Flow:
    - The seller accesses the registration form on TheEyesHaveIt.com.
    - The seller enters their physical address, telephone number, and email address.
    - The system validates the information.
    - The system creates an account for the seller.
    - The system sends a confirmation email to the seller.

**Alternate Flow:**
- If the information is invalid, the system displays an error message and prompts the seller to correct the information.


Use Case 2: Record a Book Order
- Use Case Name: Record a Book Order
- Actors: Buyer, Seller, System
- Preconditions:
    - The buyer must have an account with a valid credit card.
    - The seller must have listed books for sale.
- Postconditions:
    - The book order is recorded in the system.
    - The seller is notified of the sale.
- Main Flow:
    - The buyer searches for a book using the search engine.
    - The buyer selects a book and initiates the purchase.
    - The system prompts the buyer to log in or create an account.
    - The buyer enters payment information and confirms the order.
    - The system records the order and sends an email notification to the seller.
    - The system marks the book as sold.

**Alternate Flow:**
- If the payment fails, the system displays an error message and prompts the buyer to re-enter payment information.


# The CRUD Table

| Use Case            | Create | Read   | Update | Delete |
|---------------------|--------|--------|--------|--------|
| Add Seller          | ✔      |        |        |        |
| Record a Book Order | ✔      | ✔      |        |        |
| List Books          |        | ✔      |        |        |
| Update Book Listing |        |        | ✔      |        |
| Delete Book Listing |        |        |        | ✔      |
| Notify Buyer        |        | ✔      |        |        |
| Process Payment     |        |        |        | ✔      |

# Explanation

**Add Seller**
- Create (✔️): This use case involves creating a new seller account in the system. When a seller registers, their information is added to the database.
- Read, Update, Delete: These operations are not applicable here because the primary function of this use case is to create a new seller.
-  a Book Order
- Create (✔️): When a buyer places an order, a new order record is created in the system.
- Read (✔️): The system reads the buyer's and book's information to process the order.
- Update, Delete: These operations are not directly applicable in this use case as it primarily focuses on creating and reading data.

**List Books**
- Read (✔️): This use case allows users to view the list of available books in the system. It does not involve creating, updating, or deleting records.

**Update Book Listing**
- Create (✔️): This indicates that a seller can create or modify the details of their book listings.
- Update (✔️): This operation is applicable as sellers can update the information of their existing book listings (e.g., price, condition).
- Read, Delete: These operations are not applicable in this context.

**Delete Book Listing**
- Delete (✔️): This use case allows sellers to remove their book listings from the system if they no longer wish to sell them.
- Create, Read, Update: These operations are not applicable here.

**Notify Buyer**
- Read (✔️): This use case involves reading the buyer's information to send notifications about their order status.
- Create, Update, Delete: These operations are not applicable in this context.

**Process Payment**
- Delete (✔️): This indicates that if a payment is canceled or fails, the order may be removed from the system.
- Create, Read, Update: These operations are not applicable in this context.

**Summary**
- The checkmarks (✔️) in the CRUD table indicate which operations are relevant to each use case. This structure helps clarify the interactions between the use cases and the underlying data management processes within TheEyesHaveIt.com Book Exchange. By organizing the information this way, it becomes easier to understand the functionality required for the system and ensures that all necessary data operations are accounted for in the design and implementation phases.


## Summary
- The use case descriptions outline the processes for adding a seller and recording a book order.
- The CRUD table summarizes the operations associated with each use case, indicating which actions can be performed.


# References

- Fuchs, G., Acriche, Y., Hasson, I., & Petrov, P. (2020). Intent-Driven similarity in E-Commerce listings. ACM Digital Library. https://doi.org/10.1145/3340531.3412715
- How To Write a Product Description (Examples + Template). (2024, April 8). Shopify. https://www.shopify.com/blog/8211159-9-simple-ways-to-write-product-descriptions-that-sell
- How to Write a Use Case for Products (+ Template). (2024, August 16). Shopify. https://www.shopify.com/blog/what-is-a-use-case Indeed Editorial Team. (2023, March 11). Use Cases: What They Are and a List of Examples.
- Indeed. https://www.indeed.com/career-advice/career-development/list-of-use-cases-examples
- Jones, A. (2024, March 14). A Seller’s Guide to Writing Product Descriptions. Nimbuspost. https://nimbuspost.com/uk/blog/a-sellers-guide-to-writing-product-descriptions/
- Novgorodov, S., Guy, I., Elad, G., & Radinsky, K. (2019). Generating Product Descriptions from User Reviews. ACM Digital Library. https://doi.org/10.1145/3308558.3313532
- Novgorodov, S., Guy, I., Elad, G., & Radinsky, K. (2020). Descriptions from the Customers. ACM Transactions on Internet Technology, 20(4), 1–31. https://doi.org/10.1145/3418202 Patterson, L. (n.d.).
- Transforming a “Use Case” Into a Sales Tool. MarketingProfs. https://www.marketingprofs.com/7/transforming-use-case-into-sales-enablement-tool-patterson.asp
- What is a Use Case? How to Write One, Examples & Template | Figma. (n.d.). Figma. https://www.figma.com/resource-library/what-is-a-use-case/
