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


## Summary
- The use case descriptions outline the processes for adding a seller and recording a book order.
- The CRUD table summarizes the operations associated with each use case, indicating which actions can be performed.
