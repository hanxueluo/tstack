# Tstack


Tstack wraps gdb around, borrowing the idea from **pstack**.It logs callstack of specified function of running program. 

##How to use

###Call below command to start:

```Shell
./tstack $PID $FUNC
```

$PID is the pid of the program. $FUNC is the function name you want to trace.

###Use Ctrl+C to Stop.