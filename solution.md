1. Your main function should look like this:

```dart
void main() {
  int num1 = 3;
  int num2 = 5;
}
```

2. Create a `enum` called `Operation` outside you main function:

```dart
enum Operation {}
void main() {
  int num1 = 3;
  int num2 = 5;
}
```

3. Assign this `enum` the values plus, minus, multiply, divide:

```dart
enum Operation {
  plus,
  minus,
  multiply,
  divide,
}
```

4. Create a variable called `op` and assign it to `Operation.minus` for example:

```dart
void main() {
  int num1 = 3;
  int num2 = 5;
  const op = Operation.minus;
}
```

5. Create your `switch` statement:

```dart
void main() {
  int num1 = 3;
  int num2 = 5;
  const op = Operation.minus;
  switch (op) {}
}
```

6. Add your first case:

```dart
  switch (op) {
    case Operation.plus:
      print(num1+num2);
      break;
  }
```

7. Add the remaining cases:

```dart
  switch (op) {
    case Operation.plus:
      print(num1+num2);
      break;
    case Operation.minus:
      print(num1-num2);
      break;
    case Operation.multiply:
      print(num1*num2);
      break;
    case Operation.divide:
      print(num1/num2);
      break;
  }
```

### 🍋 Can't Divide Zero!

Add an if statement in the last case to make sure that num2 is'nt equal to zero:

```dart
    case Operation.divide:
      if(num2 == 0){
        print("Error");
    } else {
      print(num1/num2);
      }
      break;
```

