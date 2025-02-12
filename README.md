## Testbench
```
    rm WORK/*
    
    ghdl -i --ieee=synopsys -fexplicit --workdir=WORK *.vhd

    ghdl --gen-makefile --ieee=synopsys -fexplicit --workdir=WORK testbench  > Makefile

    make

    ./testbench --stop-time=500ns --wave=test.ghw

    gtkwave test.ghw &
```