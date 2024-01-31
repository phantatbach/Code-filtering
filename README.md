A simple task where I have to detect codes from strings.

Steps:
1. Use a sliding window of 10 characters to loop through the text
2. If >= 4 characters in a sliding window are special characters (e.g., @, #, ', etc), then it is likely that there are codes in that string.

Optimisation if anyone interested in using it:
1. Instead of looping character by character, you can jump straight to the next 'special character'
2. When the criterium is satisfied, the whole string will be flagged, even when the string could be really long and the code is just a tiny part of it.
   You could count the number of code_detected_times in a string then decide the cut-off point.
