# Unit Test

## Contents
- [Contents](#contents)

## General

## Write Tests First (Red Green Refactor)
General best practice is to write the test first, before wrtiing the method to be tested, so that you have proved the method works. The tests whould fail before is succeeds. The danger in not writing the test first is that the method may be initially function incorrectly unbeknownest to the developer and the test is then created based on the incorrect funtioning of the method.


## Conventions
- Test libraries should be in the form of "`[Library to be tested].Tests`"
   - ex: `MyLibrarby.Tests`
- Test class names should be in the form "`[Name of class to be tested]Tests`"
   - ex: `CalculatorTests`
- Test methods should be in the form "`[Method Name]_[Assertion]`"
   - ex: `Add_SimpleValuesShouldCalculate()`
- Variable name for the value that should be expected outcome of the test should be `expected` or variation
   - `expected`
   - `expectedSum`
   - `expectedEmail`
   - `expectedMessage`

## Parts of a Unit Test Method

The three parts of a unit test are:
- Arranage
- Act
- Assert

Arrange is where we perfom the setup actions neccessary for the test. This can include things like setting variables for expected outcone of the method being tested.

Act is where we perform the action being tested

## References
- [Intro to Unit Testing in C# using XUnit](https://www.youtube.com/watch?v=ub3P8c87cwk)
