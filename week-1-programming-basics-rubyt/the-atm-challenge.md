## Ruby basics - ATM Challenge

### Learning experience

* Review fundamentals learned in the prep course
* Learn about Ruby classes, modules, methods and attributes
* Learn about unit testing with RSpec and the benefits of writing automated tests
* Learn about naming standards
* Learn about using double, class\_double and instance\_double
* Learn about debugging and common techniques
* Work with user stories
* Learning how to pair program

### The challenge

Our client is a financial institution that wants to allow its customers to withdraw funds from their accounts using an Automatic Teller Machine \(ATM\). They have turned to us for a prototype of a system with limited functionality. Our job is to write a simple Ruby program that can be run in the Interactive Ruby Shell \(IRB\).

**You will be working with your Coach and your peers to get started with using RSpec as a testing framework an with implementing your code.**

### Scope

The following objectives must be met:

* An ATM machine can hold up to $1000
* Withdrawal can be cleared only if 
  * The ATM holds enough funds
  * The amount is divisible by 5
  * the person attempting the withdrawal provides a valid ATM card
    * Valid pin and expire date
    * Card status must be active \(Not report stolen or lost\)
  * the person attempting the withdrawal has sufficient funds in his account
* There are only $5, $10 and $20 bills in the ATM. Withdrawals for amounts not divisible by 5 must be rejected.
* Upon a successful withdrawal the system should return a receipt with information about the date, amount and bills that was dispatched. \(The receipt should be presented in the form of a Hash

#### Example output

```ruby
# Message on successful withdrawal
{ status: true, message: 'success', date: '2016-01-30', amount: 35, bills: [20,10,5]}

# Error message - wrong pin
{ status: false, message: 'wrong pin', date: '2016-01-30'}

# Error message - expired card
{ status: false, message: 'card expired', date: '2016-01-30'}
```

## Tips and Tricks

* Don't overdo it. Keep your implementation as simple as possible.
* Test your code - both manually in IRB but, most importantly with automated tests.
* You have to examine all tests ** **_**before**_** ** you write your production code. See tests as a blueprint for your implementation.
* **Run one test at the time to avoid a massive output in your terminal.** Disable `it` blocks by adding  an `x` before \(as in `xit "Should..." do`\)
* Make sure to **commit often** and \(if you are Pair Programming\) switch navigators \(the person that writes code\).

This is a good time to read the [Naming Standards](../extras/naming_standards.md) section.

