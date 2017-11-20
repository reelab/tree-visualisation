# tree-visualisation
A Python program to zoom/pan through phylogenetic trees structured by ivy

(Really large files may take long to load. I am still working to improve efficiency.)

Dependencies:
  ivy - a python library for phylogenetics: https://github.com/rhr/ivy 
  
  PyQTGraph 0.10.0 - a python library for graphics programming: https://github.com/pyqtgraph/pyqtgraph 
  
  NumPy - a python library for mathematical operations: https://github.com/numpy/numpy 
  
  Note: Please ensure you also have installed the dependencies for ivy mentioned in its documentation
    (numpy scipy matplotlib biopython pyparsing)
    
Usage:
  Run the run_tree program in ipython with an argument for the newick format tree file. Some file examples are in the examples folder.
  
    example: run run_tree examples/primates.newick
    
    If tree file is invalid or not provided a sample tree will be loaded by default. 
  
  Functions:
    Canopy Zoom mode: the center for zooming will be at the X-coordinate of mouse position and Y coordinate of tree canopy,
    
    Normal Zoom mode center: the center for zooming will be at the X and Y coordinates of mouse position,
    
    Depending on tree information provided:
      Set Node Ages: Recalculate plot so that the Y coordinates of the nodes can be set as their ages,
      Set Branch Lengths: The atual lengths of the branches can be displayed
        
  Mouse and Keyboard:
  
    Right Mouse Click: Fits the entire tree into the current window.
        Note: Right click a few times if changing modes/setting ages or lengths causes some branches to be out of bounds
        
    Mouse Wheel: Both X and Y axis zoom in and out
    
    Shift + Mouse Wheel: Only X axis zoom in and out
    
    Ctrl + Mouse Wheel: Only Y axis zoom in and out
    
    Mouse Drag: Both X and Y panning in Normal Zoom mode/ only X panning in Canopy Zoom mode
  


