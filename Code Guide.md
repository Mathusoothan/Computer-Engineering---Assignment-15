#Code Guide

C++
#include <iostream>

int main() {
  // This line prints a message to the console in C++
  std::cout << "Hello, world!" << std::endl;

  /*
  This is a multi-line comment in C++
  It can span multiple lines and is often used to provide
  more detailed explanations or information about the code.
  */
  return 0;
}

Python 

/* multiple lines */ 
// single line comment


C++
// File: main.cpp
#include <iostream>
#include "math.h"  // include the math.h header file

int main() {
  std::cout << "The square root of 4 is: " << square_root(4) << std::endl;
  return 0;
}

// File: math.h
#ifndef MATH_H  // guard against multiple inclusion
#define MATH_H

double square_root(double x);  // function declaration

#endif  // MATH_H

// File: math.cpp
#include "math.h"
#include <cmath>

double square_root(double x) {
  return std::sqrt(x);  // use the sqrt function from the cmath library
}

Python
# File: main.py
import math  # import the math package

def main():
  print("The square root of 4 is:", math.sqrt(4))

if __name__ == "__main__":
  main()

 import statement is used to import the math package, which provides a number of mathematical functions such as sqrt. The sqrt function is then used to calculate the square root of the number 4.


C++
Class
#include <iostream>

class Circle {
 public:
  Circle(double radius) : radius_(radius) {}

  double area() {
    return 3.14 * radius_ * radius_;
  }

 private:
  double radius_;
};

int main() {
  Circle circle(5);
  std::cout << "The area of the circle is: " << circle.area() << std::endl;
  return 0;
}


C++ 
Custom functions 


#include <iostream>

double square(double x) {
  return x * x;
}

int main() {
  std::cout << "The square of 4 is: " << square(4) << std::endl;
  return 0;
}


Python 
Class

class Person:
  def __init__(self,race,sex,age):
    self.Race = race
    self.Sex = sex
    self.Age = age
    print("race: {}, Breed: {},Sex: {}".format(self.Race,
                                             self.Sex,self.Age))


Python
Custom functions 

def greet(name):
  print("Hello, " + name + "!")

def main():
  greet("John")
  greet("Mary")

if __name__ == "__main__":
  main()

C++ (has a loop)

#include <iostream>

void print_numbers(int start, int end) {
  for (int i = start; i <= end; i++) {
    std::cout << i << " ";
  }
  std::cout << std::endl;
}

int main() {
  int start, end;
  std::cout << "Enter start and end values: ";
  std::cin >> start >> end;
  print_numbers(start, end);
  return 0;
}

Python has a input loop

def print_numbers(start, end):
  for i in range(start, end + 1):
    print(i, end=' ')
  print()

def main():
  start = int(input("Enter start value: "))
  end = int(input("Enter end value: "))
  print_numbers(start, end)

if __name__ == "__main__":
  main()



