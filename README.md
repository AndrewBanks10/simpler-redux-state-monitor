# simpler-redux-state-monitor

This state monitor only works for webpack managed projects and in development mode only. Ir records all simple-redux state changes. You can click on any state change in the monitor and a details div will be displayed that shows the source module, line number that caused the change and the exact state changes made.

If you use vscode then combine this monitor with the vscode extension [simpler-redux-show-state-change](https://github.com/AndrewBanks10/simpler-redux-show-state-change).

After displaying the state change details, go to vscode and open the command palette in vscode and find the command "Simpler-redux show state change". Select it. This will open the source file that caused the state change at the particular line number with highlighting on the code line. 

## Requirements

1. [simpler-redux](https://github.com/AndrewBanks10/simpler-redux)

## Usage

1) Import reducerKey and reducer from ./StateMonitor/index.js and install these in your global reducers object.
2) Import the react component exported as default from ./StateMonitor/index.js and install it your react tree.
3) The monitor does not display nor record state changes in production mode.
4) To turn off the monitor, set displayMonitor = false in ./StateMonitor/model.js  
