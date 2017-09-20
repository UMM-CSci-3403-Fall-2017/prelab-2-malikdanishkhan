# Leak report

Memory errors were present because memory allocated for the characters was never released. This was achieved by calling `free` on `result` right before the method strip returns result.
