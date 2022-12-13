DFBA
============

DFBAlab is a toolbox from MIT group.

***STEP 1*** ***Wrap the coordinates from XDATCAR***

When output XDATCAR using ASE package, the coordinates will be automatically wrapped back to the unit cell.

```python
# Wrap Li and fix O, Ti and La in the raw XDATCAR files using ASE
for i in range(mdrun):
    xdatcar = read("./xdatcar_files_raw/XDATCAR_" + str(i + 1), format='vasp-xdatcar', index=':')
    # Fix the O, Ti and La atoms
    for s in range(len(xdatcar)):
        for oi in range(len(O_coord)):
            xdatcar[s].positions[O_index[oi]] = O_coord[oi]
        for tii in range(len(Ti_coord)):
            xdatcar[s].positions[Ti_index[tii]] = Ti_coord[tii]
        for lai in range(len(La_coord)):
            xdatcar[s].positions[La_index[lai]] = La_coord[lai]
    # Write the new wrapped XDATCAR file
    write("./xdatcar_files_wrap/XDATCAR_" + str(i + 1), format='vasp-xdatcar', images=xdatcar)
    print("XDATCAR_" + str(i + 1) + " is wrapped, fixed and duplicated.")
```
