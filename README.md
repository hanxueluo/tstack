
# Tstack


Tstack wraps gdb around, borrowing the idea from **pstack**.It logs callstack of specified breakpoint of running program. 

##How to start

- Simply use the tstack like command below:

```Shell
./tstack $PID $BREAKPOINT
```

where \$PID is the pid of the program. \$BREAKPOINT is the point you want to trace. It can be a function name or code line. It's just what means in gdb.

- Use the tstack to trace multiple beakpoints:

```Shell
./tstack $PID $FUNCTIONNAME1 $FILENAME:$LINENUMBER ...
```
- trace on condition:

```Shell
./tstack $PID "$BREAKPOINT if $CONDTION" ...
```

A condition is just a gdb condition expression for breakpoint.

###Use Ctrl+C to Stop.