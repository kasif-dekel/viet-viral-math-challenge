# vietnamese-math-challenge
A viral math challenge in Vietnam: fill in the blanks with numbers from 1 to 9 to give the result 66.
http://www.mirror.co.uk/news/world-news/can-you-solve-mind-boggling-maths-5732642


# the challenge
![alt tag](http://i3.mirror.co.uk/incoming/article5732309.ece/ALTERNATES/s615/Puzzling-Puzzle.jpg)

# solution

``` python
import itertools
import sys
for combination in itertools.permutations((1,2,3,4,5,6,7,8,9)):
	if (combination[0] + ((13 * combination[1]) / combination[2]) + combination[3] + (12 * combination[4]) - combination[5] - 11 + ((combination[6] * combination[7]) / combination[8]) - 10) == 66:
		print combination
		sys.exit(1)
```
