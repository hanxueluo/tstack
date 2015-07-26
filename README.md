
# Tstack


Tstack wraps gdb around, borrowing the idea from **pstack**.It logs callstack of specified breakpoints of running program. 

##How to start

- Simply use the tstack command as below:

```Shell
./tstack $PID $BREAKPOINT
```

where \$PID is the pid of the program. \$BREAKPOINT is the point you want to trace. It can be a function name or location of code, just same with what means in gdb.

- Use the tstack to trace multiple beakpoints:

```Shell
./tstack $PID $FUNCTIONNAME1 $FILENAME:$LINENUMBER ...
```
- trace on condition:

```Shell
./tstack $PID "$BREAKPOINT if $CONDITION" ...
```

A condition is just a gdb condition expression for breakpoint.

###Use Ctrl+C to Stop.
