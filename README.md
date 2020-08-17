# Data Science Practice Daily Checkpoint

This assignment is designed to test your understanding of the daily checkpoint process. It covers:

 - Anwering a code question
 - Answering a short answer question
 
Read the instructions carefully. You will be asked both to write code and to respond to a short answer question.

**Note on daily checkpoint short answer questions:** Please use your own words. The expectation is that you have not copied and pasted from an external source, even if you consult another source to help craft your response. While the short answer questions are not necessarily being assessed on grammatical correctness or sentence structure, you should do your best to communicate yourself clearly.

## Imports

You will usually have to import different packages into a checkpoint or other material we give you

Don't worry if you don't have all the mechanics about what that means at this point

Just run the cell below, which allows the test code to function


```python
#Run this cell without changes to import tests
from test_scripts.test_class import Test
test = Test()
```

## Question 1

Copy and paste the given `greet_user` code into a cell below.

Adapt the function to do the following:

 - take a name as an argument
 - print "Greetings! I am `name` and I am pleased to make your acquaintance!"

Then in the next cell, assign the name "Gene Hackman" to the variable `name`.

Run all cells to confirm the result.


```python
# Copy / paste this starter code into a cell below
# Modify the code in this cell to use in your answer
# (Replace None with appropriate code)

def greet_user(name):
    """
    this function takes a string name as an argument 
    and prints a greeting including that name 
    """
    
    statement = None
    
    print(statement)
    
    return statement

```


```python
# Copy / paste this code into a cell below
# Modify the code in this cell to use in your answer 
# (Replace None with appropriate code)

name = None
```


```python
# Run this cell without changes to check your answer
greet_user(name)
```


```python
### BEGIN SOLUTION


def greet_user(name):
    """
    this function takes a string name as an argument 
    and prints a greeting including that name 
    """
    statement = f"Greetings! I am {name} and I am pleased to make your acquaintance!"
    print(statement)
    
    return statement

name = "Gene Hackman"

test.save(greet_user(name), 'gene_hackman')

test.save(greet_user('Ben'), 'hard_coding')

test.save(greet_user.__code__.co_varnames, 'attributes')



### END SOLUTION
```

    Greetings! I am Gene Hackman and I am pleased to make your acquaintance!
    Greetings! I am Ben and I am pleased to make your acquaintance!



```python
### BEGIN HIDDEN TESTS


test.run_test(greet_user(name), 'gene_hackman')    

name = 'Ben'
test.run_test(greet_user(name), 'hard_coding')

test.run_test(greet_user.__code__.co_varnames, 'attributes')


### END HIDDEN TESTS
```

## Question 2

Please explain the purpose of daily checkpoints and code challenges in the Flatiron School Data Science program.

=== BEGIN MARK SCHEME ===

"""The purpose of assessments are to assess a student's comprehension and application of our Data Science program's key content.
Daily checkpoints are formative, in-depth assessments
Code challenges are summative, end-to-end assessments"""

=== END MARK SCHEME ===
