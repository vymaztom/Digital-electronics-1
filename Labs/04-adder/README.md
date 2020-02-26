
## Preparation tasks (done before the lab at home)

1. A half adder has two inputs A and B and two outputs Carry and Sum. Comlpete the half adder truth table. Draw a logic diagram of both output functions.

    | **B** | **A** | **Carry** | **Sum** |
    | :-: | :-: | :-: | :-: |
    | 0 | 0 | 0 | 0 |
    | 0 | 1 | 0 | 1 |
    | 1 | 0 | 0 | 1 |
    | 1 | 1 | 1 | 0 |

2. A full adder has three inputs and two outputs. The two inputs are A, B, and Carry input. The outputs are Carry output and Sum. Comlpete the full adder truth table and draw a logic diagram of both output functions.

    | **Cin** | **B** | **A** | **Carry** | **Sum** |
    | :-: | :-: | :-: | :-: | :-: |
    | 0 | 0 | 0 | 0 | 0 |
    | 0 | 0 | 1 | 0 | 1 |
    | 0 | 1 | 0 | 0 | 1 |
    | 0 | 1 | 1 | 1 | 0 |
    | 1 | 0 | 0 | 0 | 1 |
    | 1 | 0 | 1 | 1 | 0 |
    | 1 | 1 | 0 | 1 | 0 |
    | 1 | 1 | 1 | 1 | 1 |

3. Find the relationship between half adder and full adder logic diagrams.

![img_4](../../img/04-halfAdder.gif)
![img_4](../../img/04-fullAdder.gif)

4. See schematic of the [CPLD expansion board](../../Docs/cpld_expansion.pdf) and find out the connection of LEDs, push buttons, and slide switches.

```vhdl
#-----------------------------------------------------------------------
# Buttons & switches
#-----------------------------------------------------------------------
# Two push buttons
NET BTN1        LOC = P94;
NET BTN0        LOC = P143;

# Two slide switches
NET SW1         LOC = P124;
NET SW0         LOC = P39;

#-----------------------------------------------------------------------
# Four discrete LEDs
#-----------------------------------------------------------------------
NET LD3         LOC = P64;
NET LD2         LOC = P66;
NET LD1         LOC = P68;
NET LD0         LOC = P69;
```
