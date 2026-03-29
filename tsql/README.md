# TSQL

## Unsorted Notes

What Is a Deadlock?
A deadlock occurs when two or more transactions are waiting for each other to release locks — creating a circular dependency where neither can proceed.

Simple Analogy
Imagine two people:

Person A holds a pen and wants a pencil.
Person B holds a pencil and wants a pen.
Both wait forever — deadlock.

Deadlock Prevention Checklist
Lock resources in consistent order — most important.
Keep transactions short — minimize lock duration.
Use appropriate isolation levels — READ COMMITTED by default.
Use NOLOCK for read-only queries — avoid unnecessary locks.
Implement retry logic — handle deadlocks gracefully.
Avoid nested transactions — use savepoints instead.
Use timeouts — prevent indefinite waiting.
Monitor for deadlocks — log and alert on deadlock events.

Common Pitfalls
Inconsistent lock order — causes deadlocks.
Long transactions — increase deadlock risk.
Using SERIALIZABLE — overkill, causes deadlocks.
Not retrying on deadlock — transaction fails permanently.
Ignoring deadlock errors — system becomes unreliable.