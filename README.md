# DATABASE-TRANSACTION-AND-SCID-PROPERTIES

Database Transaction
A transaction is logical unit of work which has a complete status performed within a database management system. It should not be in an inconsistent status.Example :-
Assume a user has a savings account having 4000 unit of currency. He withdraws 100 unit of currency from an ATM and this withdrawal is referred as a transaction.1. User/Card/Account authentication.
2. Withdrawal request for 100 unit of currency.
3. Balance verification.
4. Dispenses the currency to user and update the balance to 3900.
5. Print receipt and exit.
Assume that a network error happened after Step 3. The transaction will not be completed.

ACID properties
A database transaction must follow ACID properties.

A – Atomic
C – Consistent
I –  Isolated
D – Durable

Atomic :-
This property ensures the transaction either in complete status or nothing has started. There must not be any scenario like user received some currency amount and balance remains same or balance updated and failed to dispense the amount.

Consistent:-
Every transaction must be consistent.

Isolated:-
Every transaction must be isolated to avoid the locks or deadlocks. Deadlock is a condition when two or more users or processes waiting for the other to release a resource.

Durable:-
A transaction which has committed or saved must be there for permanently.
