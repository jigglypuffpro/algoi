# Cash Flow Minimizer System

## Overview
A C++ application that optimizes financial transactions between multiple banks using different payment methods. The system minimizes the number of transactions required to settle all debts by implementing a greedy algorithm with graph theory concepts.

## Features
- **Multi-Bank Support**: Handles transactions between multiple banks with different payment capabilities
- **Payment Method Optimization**: Automatically selects optimal payment methods for transactions
- **World Bank Intermediary**: Uses a central bank as intermediary when banks have no common payment methods
- **Transaction Minimization**: Reduces complex debt networks to minimum required transactions
- **Circular Debt Resolution**: Efficiently handles and optimizes circular debt patterns

## Algorithm
The system uses a greedy approach combined with graph algorithms:
1. **Net Amount Calculation**: Computes each bank's net debt/credit position
2. **Optimal Matching**: Finds best creditor-debtor pairs with common payment methods
3. **Intermediary Routing**: Routes incompatible transactions through World Bank
4. **Transaction Optimization**: Eliminates redundant and circular transactions

## Technical Implementation
- **Language**: C++ with STL
- **Data Structures**: Adjacency matrices, sets, hash maps, vectors
- **Algorithms**: Greedy optimization, graph traversal, set intersection
- **Complexity**: O(n²) time complexity for n banks

## Input Format
```
Number of banks
For each bank: Name, Payment_methods_count, Payment_methods...
Number of transactions
For each transaction: Debtor_bank, Creditor_bank, Amount
```

## Example Usage
```cpp
// Input
3
WorldBank 3 PayPal Venmo CashApp
BankA 2 PayPal Venmo  
BankB 1 PayPal
2
BankA BankB 100
BankB WorldBank 50

// Output: Optimized transaction flow
BankA pays Rs50 to WorldBank via PayPal
```


## Key Benefits
- Reduces transaction costs and processing time
- Handles real-world banking constraints (payment method compatibility)
- Scalable solution for complex multi-bank networks
- Eliminates unnecessary intermediate transactions



## Author
Shrey Chandra
<3
