  # Lab-5-Two-Points & Static Methods

In this lab, you will practice writing **static methods**, calling methods from within other methods, returning values, and formatting output.

---

## Instructions

- Start your program with your **standard header comments** (name, date, course, etc.).

-  Write a Java class with the following **four static methods**.  
   Be sure to include comments for each method.  Comments should include:
   - Description
   - Parameters
   - Preconditions
   - Postconditions
---
I have included the sample documentation for the slope method.

### Method Requirements

```java
/**Returns the slope of the line through (x1, y1) and (x2, y2).
  Precondition: x1 not equal to x2
  Postcondition:  returns a double representing the slope = (y2 - y1) / (x2 - x1)
 * @param x1 the x-coordinate of the first point
 * @param y1 the y-coordinate of the first point
 * @param x2 the x-coordinate of the second point
 * @param y2 the y-coordinate of the second point
 * @return the slope of the line through the two points
*/
public static double slope(int x1, int y1, int x2, int y2)


/**doumentation  */
public static String midpoint(int x1, int y1, int x2, int y2)

/** documentation  */
public static double distance(int x1, int y1, int x2, int y2)


/** documentation  */
public static String equationOfLine(int x1, int y1, int x2, int y2)
```

- Your `main()` method should:
  1. Ask the user to enter two points `(x1, y1)` and `(x2, y2)` as integers.
  
    Example input:

     Enter x1: 8

     Enter y1: 9

     Enter x2: 2

     Enter y2: 4


  2. Call your four methods  (passing the values/arguments)
  
  3. Print the results clearly
        - All decimal results should be rounded to 2 decimal places.  (You can use any method of rounding that you know so far.)
        - The midpoint method should return a string in the format `"(x, y)"`.
        - The equationOfLine should return the equation in the form `"y = mx + b"`
     
### Example Run

If the user enters `(8, 9)` and `(2, 4)`:

The slope is 0.83

The distance is 7.81

The midpoint is (5.0, 6.5)

The equation of the line is y = 0.83x + 2.33

### Notes
- Your code must work for **any two valid points** (except where the slope is undefined).  
- Be sure to include **preconditions**, **postconditions**, and **Javadoc-style comments**.  
- You must **call methods from within other methods** where required (e.g., `equationOfLine` must call `slope`).  
