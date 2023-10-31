# Calculator Python using SOLID

This little project's main goal was to practice OOP, SOLID, design patterns and RESTful API with Flask and Python. It also includes some Unit Testing with "unittest" library.

- Run:
  You must give permissions to the script with the following command:

```
chmod +x run.sh
```

Now you can run the project with the following:

```
./run.sh
```

The output will instruct you to open `http://127.0.0.1:5000`, from there you can send HTTP requests with the desired input to the project, on path `http://127.0.0.1:5000/(mathematical-expression)/(extension)`.

For example:

```
http://127.0.0.1:5000/5+3
```

- The server will take care of the rest.

The only extension implemented ATM is "color" which will result with returning a JSON containing the result of the "mathematical-expression" and a color: green if the result is even, or red if it is odd. Of course, the main goal of that is to show that implementing new extensions and mathematical operations is possible while adhering to SOLID and not violating it (mainly regarding the Open/closed principle).

- Please do note that the division sign should be " : " and not " / " .

# Test

To run the tests you need to navigate to the `calculator-python` folder:

```
cd calculator-python
```

Now run:

```
python3 -m unittest unit_testing.py
```

- A dot (.) indicates a test that has successfully passed.
- An F indicates a test that has failed (will be shown alongside with the given failure text message set in the testing function)."
- An E indicates a test that couldn't run due to an error (will be shown alongside with the error message).
