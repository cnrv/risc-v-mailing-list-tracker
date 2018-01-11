# Optional performance monitors implementation

link: [see here](https://groups.google.com/a/groups.riscv.org/d/msgid/isa-dev/BY2PR0401MB10615E41189408BA3395C75DFB110%40BY2PR0401MB1061.namprd04.prod.outlook.com?utm_medium=email&utm_source=footer)

start time: 01-11-2018

end time: 01-11-2018

## Related to (tag)

- Implementation
- Emulation
- Hardware performance monitor (3.1.16 of privspec)

## Background


## Questions

Joe asked:" Version 1.11 of the privileged architecture document does not explicitly state whether mcycle and minstret must be implemented. Can someone please clarify this issue?
Section 3.1.16 (relevant part copied below) states that “All counters should be implemented”. Is an illegal instruction exception that is handled by software to return zero an acceptable implementation? Or, are the performance monitoring counters required to return zero without an exception for them to be considered legal?"



## Discussion

But why couldn't we use exception or emulation?
What do we mean by "should be implemented"?
How to test it in compliance test?


## Solutions
Should return 0. It couldn't fail or use exception.

## Summary


## Additional discussion

