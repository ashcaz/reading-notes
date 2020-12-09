# Testing and Modules

**LINKS**

- [In Tests We Trust - TDD with Python](hhttps://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)
- [Recursion](https://www.geeksforgeeks.org/recursion/)
- [Video:Python Modules and Packages Companion Video](https://realpython.com/courses/python-modules-packages/)
- [Google for Education: Python Lists](https://developers.google.com/edu/python/lists)
- [Google for Education: Python Strings](https://developers.google.com/edu/python/strings)
- [Python Modules and Packages](https://realpython.com/python-modules-packages/)
- [Pytest Documentation](https://docs.pytest.org/en/latest/)
- [PyTest Tutorial Up to section `Running tests in parallel`](https://www.guru99.com/pytest-tutorial.html)

## In Tests We Trust - Test Driven Development(TDD) with Python

**AAA: Arrange, Act and Assert**

- **Arrange**: you need to organize the data needed to execute that piece of code (input)
- **Act**: here you will execute the code being tested (exercise the behaviour)
- **Assert**: after executing the code, you will check if the result (output) is the same as you were expecting

### The Cycle

The cycle is made by three steps:

- Write a unit test and make it fail 
- Write the feature and make the test pass!
- Refactor the code — the first version doesn’t need to be the beautiful one

Two books to dive into TDD:

- [Test Driven Development: By Example](https://www.amazon.com.br/Test-Driven-Development-Kent-Beck/dp/0321146530)
- [Growing Object-Oriented Software, Guided by Tests](https://www.amazon.com.br/Growing-Object-Oriented-Software-Guided-Tests/dp/0321503627)


## Recursion

### What is Recursion?
The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function.

```Python
def tri_recursion(k):
  if(k>0):
    result = k+tri_recursion(k-1)
    print(result)
  else:
    result = 0
  return result

print("\n\nRecursion Example Results")
tri_recursion(6)
```

[Real World Example of Recursion](https://stackoverflow.com/questions/105838/real-world-examples-of-recursion)

[Back to Homepage](https://ashcaz.github.io/reading-notes)

