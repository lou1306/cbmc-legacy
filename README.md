# CBMC: Legacy

This is just a fork of [CBMC 5.4](http://www.cprover.org/cbmc/)
with a few bells and whistles. 
It uses a modified MiniSat called [PlanckSat](https://github.com/lou1306/plancksat)
as the verification backend. 

This allows the user ofCBMC-Legacy to generate randomized counterexample,
guide the analysis by means of strong and weak assumptions, etc.

## Compiling

This should do the trick:

```bash
git clone git@github.com:lou1306/cbmc-legacy.git
cd cbmc-legacy
git submodule init # Downloads PlanckSat
make
```

A `cbmc` binary will show up in the `src/cbmc` directory.

