import 'dart:io';

void main() {
  stdout.write('Enter a number: ');
  String userInput = stdin.readLineSync();
  int number = int.tryParse(userInput);
  
  if (number != null) {
    if (number > 10) {
      print('Your number is greater than 10');
    } else if (number < 10) {
      print('Your number is less than 10');
    } else {
      print('Your number is equal to 10');
    }
  } else {
    print('Invalid input. Please enter a valid number.');
  }
}
