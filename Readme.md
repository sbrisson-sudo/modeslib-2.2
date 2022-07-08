# modeslib-2.2

Fast computation of seismograms in a radially symetric Earth model by Normal Modes Summation (NMS).
Quick documentation : 

- To compile the code :
    ```bash
    mkdir build
    cmake -B build
    cmake --build build
    ```

- To run the binaries :
    1. Build the mode database 
        - input file : `yannos.dat`
        - binary : `yannos`
    2. Run the normal mode summation
        - input files : `nms.dat` `source.dat` `receivers.dat` 
        - binary  : `nms`
    
Examples of the input files can be found under the `example` directory.
