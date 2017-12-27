### Travis & Coveralls

### Continuous Integration and QA

During the development process of an application or before deploying code to a server, it is very important to verify the quality of the code. Continuous Integration \(CI\) is a development practice that allows us to verify checked-in code using an automated build and to detect problems early.

[**Travis**](https://travis-ci.org/) is a continuous integration tool that, once configured, takes care of these tasks and let us save a lot of time \(that we can use to actually write code\). Travis-ci.org is an online service that works with GitHub \(it requires we use GitHub as the repository for our code\), and once we have connected the two accounts and configured a very simple file in our projects, it’s automatically triggered when we push on our GitHub repository.

[**Coveralls**](https://coveralls.io/)runs tests and checks the percentage of the source code that is covered by tests, producing a nice report that shows us the percentage for every single file/module and even the lines of code that have been tested.

