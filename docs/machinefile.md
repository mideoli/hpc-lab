# Machinefile

```
node1 slots=3
node2 slots=3
```

Run:
```
mpirun -n 6 --machinefile machinefile ./a.out
```
