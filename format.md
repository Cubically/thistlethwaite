The output will represent a Rubik's Cube, formatted how solutions to [this challenge][2] take input. This format is a bit confusing, so here's a way to visualize it. This is the solved cube:

[![solved visualization][1]][1]

That renders the output `UF UR UB UL DF DR DB DL FR FL BR BL UFR URB UBL ULF DRF DFL DLB DBR`.

If we were to swap, for example, the red-white edge and the red-blue edge, the visualization would look like this (with no changes to the hidden faces):

[![swapped visualization][2]][2]

That renders the output `UR UF UB UL DF DR DB DL FR FL BR BL UFR URB UBL ULF DRF DFL DLB DBR` (which, btw, is an impossible cube state). Note that the order of the letters in cubies matter:

    Above: UR UF UB UL DF DR DB DL FR FL BR BL UFR URB UBL ULF DRF DFL DLB DBR
    Below: RU FU UB UL DF DR DB DL FR FL BR BL UFR URB UBL ULF DRF DFL DLB DBR

[![swapped reversed visualization][3]][3]

---

A cube scrambled with `L2D2L2D2B2R2F2L2D2U2F2UF2U'R2UB2U'L2UB2U'LU'L2U'D'B2U'RBUBF'D'` creates this cube (only top, front, and right faces shown):

[![scrambled visualization][4]][4]

    Solved:    UF UR UB UL DF DR DB DL FR FL BR BL UFR URB UBL ULF DRF DFL DLB DBR
    Scrambled: RU LF UB DR DL BL UL FU BD RF BR FD LDF LBD FUL RFD UFR RDB UBL RBU

As you can see in the comparison above and in the visualizations, the blue-red `RU` edge of the mixed cube is in the place of the red-white `UF` edge of the solved cube. The green-white `LF` edge is in the place of the red-blue `UR` edge, etc.

   [1]: https://i.stack.imgur.com/bU5Nc.png
   [2]: https://i.stack.imgur.com/pdndD.png
   [3]: https://i.stack.imgur.com/mQF50.png
   [4]: https://i.stack.imgur.com/X8S81.png
