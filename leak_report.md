# Leak report

Memory errors were present because strcmp was obtaining an empty string. This was avoided by adding an `if` statement that checks for an empty string. If an empty string is present it returns false, otherwise it compares and cleans.
