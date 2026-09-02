---
Date & Time: 02-09-2026 14:19
Lecturer:
  - Tilo Burghardt
Course Name:
  - COMS10016
Lecture Name: Loops & Jumps
---
## Loops
```C
// While loop
while (t > 0) {
	sleep(1);
	t--;
}

// For Loop
for (int t = 10; t > 0; t--) {
	sleep(1);
	t--;
}
```
Remarks: Use POSIX library for better portability

## Operators
```C
n++; <=> ++n; <=> n+=1;
n--; <=> --n; <=> n-=1;

m = n++;  // m = n; n++;
m = ++n;  // n++; m = n;
```

## Jumps
🚨 <mark style="background: #FF5582A6;">Avoid</mark> using this

- Do-while loop
```C
do {
} while (t>0);

// Use
while (t>0) {
}
```

- GOTO
```C
int t = 10;
LABEL:
if (t > 0) goto LABEL;

// Use
do {} while (t>0) {}
```

- Continue
```C
for (...) {
if (!isPrime(i)) continue;
}

// Use
if (!isPrime(i)) {
}
```

- Break
```C
while (i < last) {
	break;
}
```

---
#Imperative 