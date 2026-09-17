---
Date & Time: 10-09-2026 12:21
Lecturer:
  - Tilo Burghardt
Course Name:
  - COMS10016
Lecture Name: Searching & Runtime Complexity
---
## Searching
### Linear Search
```C
int linearSearch(char c, int n, char a[n]) {
	int result = -1;
	for (int i = 0; i < n; i++) {
		if (a[i] == c) {
			return i;
		}
	}
}
```
- Iterate through each item, then compare

### Binary Search
```C
int binarySearch(char c, int n, char a[n]) {
	int start = 0, end = n, mid;
	bool found = false;
	
}
```




---
#Imperative