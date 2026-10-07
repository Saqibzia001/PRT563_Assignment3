# PRT563 Assignment 3 - Final Checklist

## Dataset and import
- 13 CSV files are present.
- Dataset matches Assignment 2 source: 10/10/10/10/10/10/10/20/20/10 for the main entity counts.
- `CONTAINS` count is 20.
- Operational graph relationship count is 150 before derived analytics relationships.
- `import.txt` is run once on a fresh dedicated Neo4j database.

## Validation
- `SHOW CONSTRAINTS` completes successfully.
- `SHOW INDEXES` completes successfully.
- Customer, Address, Store, Driver, Category, MenuItem and MenuVariant counts are 10 each.
- Order count is 20.
- Payment count is 20.
- Delivery count is 10.
- Orders 1-10 are PickupOrder and Orders 11-20 are DeliveryOrder.
- Both-subtype violation = 0.
- Delivery orders without fulfilment = 0.
- Pickup orders with fulfilment = 0.
- Invalid CONTAINS rows = 0.
- Duplicate order-line keys = 0.
- Invalid behaviour vectors = 0.

## Cypher queries
- Q1 available mid-range variants executes.
- Q2 customer orders and destination executes.
- Q3 paid store average vs global average executes.
- Q4 above-median customers using both pickup and delivery executes.

## GDS analytics
- `operationalCentrality` projection executes.
- Degree, Betweenness, Closeness and PageRank execute.
- `customerVariantSimilarity` projection executes with 20 nodes and 20 projected relationships in the final Aura evidence.
- Jaccard executes.
- `customerAffinitySimilarity` projection executes with 22 nodes and 46 projected relationships in the final Aura evidence.
- Filtered Node Similarity with Overlap executes.
- `customerSpendKNN` projection executes with 10 Customer nodes and no relationship projection.
- KNN cosine executes with `behaviourVector`.
- Genuine result screenshots are retained.

## Submission
- Final Word report is reconciled with the final repository and live evidence.
- Upload the repository contents to the permitted GitHub/OneDrive location.
- Paste the real repository URL into Blackboard where required.
- Do not upload passwords, tokens or private database files.
