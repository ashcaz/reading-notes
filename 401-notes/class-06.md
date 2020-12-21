# Random Module & Risk Analysis

**LINKS**

- [How to use Random Module](https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)
- [What is Risk Analysis](https://www.edureka.co/blog/risk-analysis-in-software-testing/)
- [Video: Big O Notation](https://www.youtube.com/watch?v=v4cd1O4zkGw)
- [Python Random](https://docs.python.org/3/library/random.html)
- [What is Dependency Injection](https://www.freecodecamp.org/news/a-quick-intro-to-dependency-injection-what-it-is-and-when-to-use-it-7578c84fa88f/)
- [W3Schools Random Modue](https://www.w3schools.com/python/module_random.asp)

## How to use Random Module

### Random Functions

**Randit**

If we wanted a random integer, we can use the randint function Randint accepts two parameters: a lowest and a highest number. Generate integers between 1,5. The first value should be less than the second.

```Python
import random
print random.randint(0, 5)
```

**Random**

The `random()` method returns a random floating number between 0 and 1.

If you want a larger number you can just multiply it:
```Python
import random
random.random() * 100
```

**Choice**

The `choice()` method returns a randomly selected element from the specified sequence. The sequence can be a string, a range, a list, a tuple or any other kind of sequence.

```Python
import random
myList = [2, 109, False, 10, "Lorem", 482, "Ipsum"]
random.choice(myList)
```

**Shuffle**

The `shuffle()` method takes a sequence (list, string, or tuple) and reorganize the order of the items.

```Python
import random

mylist = ["apple", "banana", "cherry"]
random.shuffle(mylist)

print(mylist)
```

**Randrange**

The `randrange()` method returns a randomly selected element from the specified range.

`random.randrange(start, stop, step)`


[Back to Homepage](https://ashcaz.github.io/reading-notes)