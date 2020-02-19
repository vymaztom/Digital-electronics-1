## Preparation tasks (done before the lab at home)

1. See [schematic](../../Docs/coolrunner-ii_sch.pdf) or [reference manual](../../Docs/coolrunner-ii_rm.pdf) of the board and find out the connection of 7-segment display. How can you change the position of the character on the display?

```vhdl
# LED segments
NET disp_seg_o<6>   LOC = P56;  # segment a
NET disp_seg_o<5>   LOC = P53;  # segment b
NET disp_seg_o<4>   LOC = P60;  # segment c
NET disp_seg_o<3>   LOC = P58;  # segment d
NET disp_seg_o<2>   LOC = P57;  # segment e
NET disp_seg_o<1>   LOC = P54;  # segment f
NET disp_seg_o<0>   LOC = P61;  # segment g

# Digits
NET disp_dig_o<3>   LOC = P130;
NET disp_dig_o<2>   LOC = P129;
NET disp_dig_o<1>   LOC = P128;
NET disp_dig_o<0>   LOC = P126;
```


2. Complete the decoder conversion table for common anode display.

    | **Hex** | **Input** | **a** | **b** | **c** | **d** | **e** | **f** | **g** |
    | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
    | 0 | 0000 | 0 | 0 | 0 | 0 | 0 | 0 | 1 |
    | 1 | 0001 | 1 | 0 | 0 | 1 | 1 | 1 | 1 |
    | 2 | 0010 | 0 | 0 | 1 | 0 | 0 | 1 | 0 |
    | 3 | 0011 | 0 | 0 | 0 | 0 | 1 | 1 | 0 |
    | 4 | 0100 | 1 | 0 | 0 | 1 | 1 | 0 | 0 |
    | 5 | 0101 | 0 | 1 | 0 | 0 | 1 | 0 | 0 |
    | 6 | 0110 | 0 | 1 | 0 | 0 | 0 | 0 | 0 |
    | 7 | 0111 | 0 | 0 | 0 | 1 | 1 | 1 | 1 |
    | 8 | 1000 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
    | 9 | 1001 | 0 | 0 | 0 | 1 | 1 | 0 | 0 |
    | A | 1010 | 0 | 0 | 0 | 1 | 0 | 0 | 0 |
    | b | 1011 | 1 | 1 | 0 | 0 | 0 | 0 | 0 |
    | C | 1100 | 0 | 1 | 1 | 0 | 0 | 0 | 1 |
    | d | 1101 | 1 | 0 | 0 | 0 | 0 | 1 | 0 |
    | E | 1110 | 0 | 1 | 1 | 0 | 0 | 0 | 0 |
    | F | 1111 | 0 | 1 | 1 | 1 | 0 | 0 | 0 |
