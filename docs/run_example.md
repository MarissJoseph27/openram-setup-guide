# Generating an SRAM macro


## Activate the Python Environment and Nix shell


``` bash
cd OpenRAM
source openram_env/bin/activate
nix develop
```
If the virtual environment is located elsewhere, adjust the path accordingly.

## Verify the Environment Variables 

``` bash
echo $OPENRAM_HOME
echo $OPENRAM_TECH
```
You should see the paths to your OpenRAM installation and technology directory.

## Build the Example SRAM

```bash
cd macros
make sky130_sram_1rw_tiny
```
OpenRAM will begin generating the SRAM and display messages as it progresses.

## Expected Output

When the build finishes successfully, a directory similar to the following will be created:
```bash
macros/sky130_sram_1rw_tiny/ (contains generated files)
macros/sky130_sram_1rw_tiny.ok/
```
The generated files typically include:
| File    | Description                         |
| ------- | ----------------------------------- |
| `.gds`  | Physical layout                     |
| `.lef`  | Abstract layout for place-and-route |
| `.sp`   | SPICE netlist                       |
| `.lib`  | Liberty timing model                |
| `.v`    | Verilog model                       |
| `.html` | Design summary                      |
| `.log`  | Build log                           |




