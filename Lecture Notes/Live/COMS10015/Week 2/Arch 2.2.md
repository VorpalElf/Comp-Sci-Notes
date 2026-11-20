---
Date & Time: 28-09-2026 13:11
Lecturer:
  - Daniel Page
Course Name:
  - COMS10015
Lecture Name: Integer Representation
---
## Binary Addition

![[Screenshot 2026-09-28 at 2.29.31 PM.png]]

```Python
# Assume little endian
def add_binary(x, y, n, b, ci):
	r = [0] *n
	c = ci  # Technically can name as c, but ci to demo carry input
	
	for i in range(n):
		total = x[i] + y[i] + c
		r[i] = total % 2
		if (total >= b):
			c = 1
		else:
			c = 0
			
	co = c  # co: carry out
	return r, co
```


## Overflow
- Extra bit produced after arithmetic operation
- Bit unable to fit in the register
- Actions: Truncate/clamp the result
![[Screenshot 2026-09-28 at 1.48.37 PM.png]]
Figure 1: Actions taken based on signed number arithmetic operations

---
#Binary #Architecture