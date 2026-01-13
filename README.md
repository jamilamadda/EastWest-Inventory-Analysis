
## The EastWest Inventory Analysis

EastWest is a anonymized branded apparel and merchandise agency that manages thousands of custom items for its clients. In this project, I analyzed real inventory transaction data to understand product flow, detect stock-outs, and evaluate how well the company’s current forecasting and reordering strategy performs.


**Understanding the Data**  
Inventory levels change over time as products are ordered, allocated to customers, and shipped. The TransactionType column captures these movements:  
* Allocate: Created when a customer order reserves inventory.  
    * This increases the QuantityAllocated value for that product.  
* Fulfilled: Created when a product is actually shipped to the customer.  
    * This decreases the QuantityOnHand.  
    * Each Fulfilled row is paired with an Allocation Adjustment row, which decreases Quantity Allocated.



**Key Questions to Answer**
1. Stock-Out Behavior: A stock-out occurs when QuantityOnHand becomes 0 for a product.  
* How frequently do stock-outs occur across products?  
* When they do occur, how long do they typically last? (i.e., time from hitting zero until inventory is replenished)  
* After a stock-out begins, how quickly does a reorder usually happen?  
* Once reordered, how long does it take for the product to be back in stock?

PowerBi Dashboard Link : https://app.powerbi.com/view?r=eyJrIjoiMjUxNzQxY2EtZTE5MS00MzMxLWFkYzAtODRmMDQxMmQ2ZWI0IiwidCI6IjEwMWRhNTg3LTE4NDMtNGY1Mi04YjhhLTE3YjA2OWM2NmQzMyIsImMiOjJ9