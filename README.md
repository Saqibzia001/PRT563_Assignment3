# PRT563 Assignment 4 - Neo4j Graph Database Migration

## Dataset baseline
- 10 Customers
- 10 Addresses
- 10 Stores
- 10 Drivers
- 10 MenuCategories
- 10 MenuItems
- 10 MenuVariants
- 20 Orders
- 20 Order-item rows / `CONTAINS` relationships
- 20 Payments
- 10 Deliveries
- 10 Pickup orders
- 10 Delivery orders

## Repository contents
- `import.txt` - final one-run Neo4j import, constraints, relationships, indexes and derived analytics layers.
- `queries.txt` - four Cypher use cases.
- `gds_algorithms.txt` - four centrality algorithms and three similarity experiments.
- `live_verification.txt` - migration and integrity checks.
- `csv/` - all 13 source CSV files.
- `source/Assignment2_SQL_source.sql` - Assignment 2 source SQL for traceability.

## Required CSV files
`customers.csv`, `addresses.csv`, `stores.csv`, `drivers.csv`, `categories.csv`, `menu_items.csv`, `menu_variants.csv`, `orders.csv`, `order_items.csv`, `payments.csv`, `deliveries.csv`, `pickup_orders.csv`, `delivery_orders.csv`.

## Execution order
1. Create a dedicated fresh Neo4j database for this assignment.
2. Install a compatible GDS version and confirm `RETURN gds.version();` works.
3. Copy all CSV files into the active Neo4j import directory.
4. Run the whole `import.txt` from top to bottom once.
5. Run `live_verification.txt` and confirm expected counts and zero violation counts.
6. Run Q1-Q4 from `queries.txt` separately.
7. Run the centrality and similarity sections of `gds_algorithms.txt` in order.

.




