# Qspice_CMOSedu
Qspice models for textbook - [CMOS Circuit Design, Layout, and Simulation, 3rd edition by R. Jacob Baker](https://www.amazon.com/Circuit-Design-Simulation-Microelectronic-Systems/dp/0470881321)



Qspice filetypes:

-  *.qsch: netlist schematic model
- *.qraw: raw data. (for saving all data, please use '.save all' spice code in schematic)
- *.pfg: configure file for raw data plotting
- *.cir: netlist code





## WINOS

> Every chapter folder has cmosedu_model.txt and Makefile. 
>
> In order to use 'make' command in windows OS, please install [cmder - console emulator](https://cmder.app/), and launch the terminal in the chapter folder. 



> For using qspice to simulate spice netlist file, create a new folder named Bin in the qspice installation folder. Then, copy and save *QSPICE64.exe* as *qspice.exe* in Bin folder. For plotting the *.raw data, please also copy and save *QUX.exe* as *qplot.exe* in the same Bin folder.  Add the Bin absolute directory into the Windows PATH environment. Now, open a terminal and type '`qspice spice_ex.qsch`' for spice simulation.



## LINUX

Qspice can be used in Linux after WINEHQ installation.  Add the following alias to .cshrc or .bashrc and then open a new terminal to run qspice or qplot command. 

```
> alias qspice=$QSPICE_HOME/QSPICE64.exe
> alias qplot=$QSPICE_HOME/QUX.exe
```

Qspice commands in terminal

```
> qspice spice_ex.qsch	# run the netlist
> qplot spice_ex.qraw   # plot the data
```

