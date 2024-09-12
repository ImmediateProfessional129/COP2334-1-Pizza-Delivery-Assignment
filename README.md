# COP2334-1-Pizza-Delivery-Assignment
This is a repository link of the COP2334-1 Module 3 Assignment

// This is a pizza ordering program created by Marcello Gonzalez
#include <iostream>
#include <iomanip>
using namespace std;

int main() {

  // Declaring variables
  cout << fixed << setprecision(2);

  // The variable for the customer's pizza quantity
  int quantityOfPizzas;
  // The variable for the cost of each pizza
  const double perPizzaCost = 14.99;
  // The variable for the sales tax percentage
  const int SalesTax = 8;
  // The variable for the primary cost of the pizza
  double SubTotal = 0;
  // The variable for the total cost of the pizza after tax
  double Total = 0;

  // The statement that asked the user to enter the quantity of pizzas
  cout << "How many pizzas would you like to order? ";
  // The statement that takes the user's input and stores it in the quantityOfPizzas variable
  cin >> quantityOfPizzas;
  // The statement that estimates the subtotal
  SubTotal = quantityOfPizzas * perPizzaCost;
  // The statement that assesses the total cost after tax
  Total = SubTotal + (SubTotal * SalesTax / 100);
  // The statement that displays the subtotal and total cost
  cout << "The subtotal is: $" << SubTotal << endl;
  cout << "Your total is $" << Total << endl;
  return 0;
}
