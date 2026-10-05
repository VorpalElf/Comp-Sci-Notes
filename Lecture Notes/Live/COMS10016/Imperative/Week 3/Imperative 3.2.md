---
Date & Time: 05-10-2026 15:09
Lecturer:
  - Otto Brookes
  - Tilo Burghardt
Course Name:
  - COMS10016
Lecture Name: Search
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
	
	while ((!found) && (end > start)) {
		mid = start + (end-start)/2
		if (c == a[mid]) {
			found = true;
		} else if (c < a[mid]){
			end = mid;
		} else {
			start = mid + 1;
		}
	}
	if (!found) {
		mid = -1;
	}
	return mid;
}
```

## Runtime Complexity
[![Basics of Big O Notation. I have written about algorithms in the… | by  Nicky Liu | The Startup | Medium](https://miro.medium.com/v2/resize:fit:1400/1*5ZLci3SuR0zM_QlZOADv8Q.jpeg)
- Keep the most significant term
- Discard coefficients
- E.g. $an+b \implies n$


---
#Imperative