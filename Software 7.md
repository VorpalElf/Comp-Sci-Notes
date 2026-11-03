---
Date & Time: 03-11-2026 11:13
Lecturer:
  - Matthew Edwards
Course Name:
  - COMS10012
Lecture Name: Testing
---
## Assertions
- Mechanisms for making a <mark style="background: #FFB86CA6;">logical statement</mark> about <mark style="background: #ABF7F7A6;">variables</mark> in your program
- Have access to the internal state of your program
```C
static void add_mime_mapping(const char *extension, const char *mimetype) {
    size_t i;
    assert(strlen(extension) > 0);
    assert(strlen(mimetype) > 0);
```

## Unit Testing
- Run code against a set of inputs

## Test Driven Development
- **RED**: Make a test that will fail
- **GREEN**: Make a test that will pass
- **REFACTOR**: Improve code quality, but still passes all tests

## Property Testing



---
