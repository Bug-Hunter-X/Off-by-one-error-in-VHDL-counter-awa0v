# Off-by-One Error in VHDL Counter

This repository demonstrates a common off-by-one error in a simple VHDL counter and its solution.  The `buggy_counter.vhdl` file contains the erroneous code, while `fixed_counter.vhdl` provides the corrected implementation.

**The Bug:**

The original counter fails to reset correctly when it reaches its maximum value (15). This is due to a subtle error in the conditional statement that handles the reset condition. The corrected version includes the missing semicolon to fix the error.

**The Solution:**

The solution simply corrects the assignment statement inside the `if internal_count = 15 then` block.  A missing semicolon caused a syntax error in the original code which was causing the unexpected behavior.