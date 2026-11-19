# Exercise 5: Equality Predictions (S17 homework)

Use these variables for every row:

```java
String a = "Java";
String b = a;
String c = new String("Java");
String d = "java";
String e = null;
```

**Predict first.** Fill in the Predicted column for all ten rows BEFORE you run anything. A blank prediction scores zero. For compareTo rows write only negative, zero or positive.

| # | Expression | Predicted | Actual | Missed? |
|---|---|---|---|---|
| 1 | `a == b` | True | True | No |
| 2 | `a == c` | False | False | No |
| 3 | `a.equals(c)` | True | True | No |
| 4 | `a.equals(d)` | False | False | No |
| 5 | `a.toLowerCase().equals(d)` | True | True | No |
| 6 | `a.compareTo(c)` | 0 | 0 | No |
| 7 | `a.compareTo(d)` | Negative | Negative | No |
| 8 | `"apple".compareTo("banana")` | Negative | Negative | No |
| 9 | `"b".compareTo("a")` | Positive | Positive | No |
| 10 | `a.equals(e)` | False | False | No |

Run each one in a scratch Java file and fill in Actual. Mark every miss.

## For each miss: one sentence
Say whether it was `==` versus `equals`, or the sign of `compareTo`.

-

## One safe line
Write ONE line of code that is true when `s` matches "yes" and never crashes, even if `s` is `null`.

```java
String s = null;
System.out.println("yes".equalsIgnoreCase(s));
```

## Before tomorrow
Peer code review is next class. Make sure `src/EmailParser.java` is pushed to your fork.
