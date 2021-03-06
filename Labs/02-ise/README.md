# 2. lecture (02-ise)

#### Contents

1. [Homework](#Homework)

<!--
2. [Used hardware components](#Used-hardware-components)
3. [Synchronize Git and create a new folder](#Synchronize-Git-and-create-a-new-folder)
4. [Digital circuits in VHDL language](#Digital-circuits-in-VHDL-language)
5. [Clean project and synchronize git](#Clean-project-and-synchronize-git)
6. [Ideas for other tasks](#Ideas-for-other-tasks)
-->

## Homework

1. *Binary comparator* true table.

    | **A** | **B** | **A>B** | **A=B** | **A<B** |
    | :-: | :-: | :-: | :-: | :-: |
    | 0 | 0 | **0** | **1** | **0** |
    | 0 | 1 | **0** | **0** | **1** |
    | 1 | 0 | **1** | **0** | **0** |
    | 1 | 1 | **0** | **1** | **0** |

2.   **SoP** and **PoS** output forms as follows


![equation](https://latex.codecogs.com/gif.latex?y_%7BA%3EB%7D%5E%7BSoP%7D%3D%20A%20%5Ccdot%20%5Coverline%7BB%7D)



![equation](https://latex.codecogs.com/gif.latex?y_%7BA%3DB%7D%5E%7BSoP%7D%3D%20%5Coverline%7BA%7D%5Ccdot%5Coverline%7BB%7D%20&plus;%20A%5Ccdot%20B)



![equation](https://latex.codecogs.com/gif.latex?y_%7BA%3CB%7D%5E%7BPoS%7D%3D%20%28%5Coverline%7BA%7D&plus;B%20%29%5Ccdot%20%28%5Coverline%7BA%7D%20&plus;%20%5Coverline%7BB%7D%29%5Ccdot%28A%20&plus;%20B%29)



Create K-maps for all three functions.


![basic_gates](../../img/02-tables.png)


Use the K-map to create the minimum ![equation](https://latex.codecogs.com/gif.latex?y_%7BA%3CB%7D%5E%7BPoS%2Cmin%7D) function.

&nbsp;

![equation](https://latex.codecogs.com/gif.latex?y_%7BA%3CB%7D%5E%7BPoS%2C%20min%7D%3D%20%5Coverline%7BA%7D%5Ccdot%20B)

&nbsp;

> Equations and symbols were generated by [Online LaTeX Equation Editor](https://www.codecogs.com/latex/eqneditor.php) as an Encoded URL link.
>
