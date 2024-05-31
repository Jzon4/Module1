# Module-Functions-and-Errors---ETH-AVAX

# VIDEO LINK


# SUMMARY OF THIS CODE 
This Solidity smart contract is designed to manage orders for a donut delivery service. Here's a summary:

Contract Name: MyNewContract
State Variables:
orderCount: A public unsigned integer to keep track of the total number of orders placed.
Order: A struct defining the structure of an order, containing the client's address, the donut selection (represented by an unsigned integer), and a boolean indicating whether the order has been delivered.
orders: A mapping from order numbers (unsigned integers) to Order structs, allowing retrieval of order details by order number. placeOrder: A function for placing a new order. It takes a donut selection as input and requires payment of at least 1 ether. Upon successful payment, it creates a new Order struct with the sender's address, donut selection, and delivered status set to false. It increments orderCount and stores the new order in the orders mapping.
delivered: A function for marking an order as delivered. It takes the order number as input and sets the delivered status of the corresponding order to true. Additionally, it includes an assertion to ensure that the delivered status is indeed true after setting it.
Overall, this contract provides functionality for placing orders and marking them as delivered, ensuring payment is received before accepting an order, and maintaining order details on the blockchain. Additionally, it employs some best practices like using require for input validation and assert for internal consistency checks.


## Author

Jayson C. Alejandro BSIT
@Jzon4

# LICENCE
Copyright (c) 2024 Jzon4
