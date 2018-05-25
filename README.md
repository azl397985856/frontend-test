# Frontend Test
This repo contains almost everything about frontend  testing, it's usefull especially when you'r building large apps.

It mainly cover there four parts:

* What is test

* Why to test

* Ways to test

* Visual test

> this topic only covers the test itself, and the framework parts such as mocha and jest are on their way.
## What the hell is test
Test is `code` to ensure your code works `as expected`.

To `ensure`, we may need to assert which is the core of testing.

To be `as excepected`, you may need to consider every part about your program, nobody can help you,
there is no silver bullet. But high coverage always produce hight quality code.

> alway doesn't mean inevitable
## Why to test
### To deploy your app with no fear
without testing, adding new feature or fixing bug is tough.

It's hard to guarantee the code added doesn't effect the old code.
(fix a bug, produce two or more bugs)

But things are diffrent if your code base is well tested.
sure, you can deploy your app without fear.

>  it doesn’t really matter how you do your tests, as long as you write enough tests that make you feel confident that you can deploy your version to production.          --Gil Tayar
## Ways to test
There are so many types of test.

The terminology make it more hard to understand.

Before we dive into `ways to test`.
Let's get started with the simplest - `unit test`.
### unit test
> Unit testing is code that tests units of code, whether they be functions, modules, or classes.
 
Unit tests are the easiest tests to write, and the easiest tests to understand, as they are usually functional in nature — setup a unit with input, make it do it’s thing, and check the output (where the input could be a function parameter, and the output just the return value).

Moreover, you should encourage yourself to write the code in a way that makes it possible to test those units in isolation, without needing to bring in other units.

Code that is perfect for unit-testing is code that has no I/O or UI dependencies.
if you do(actually you did), try mock. More advance, try to limit the side effect(here is IO and UI) into a small area, 
functional programming is good at it.

### integration test
also, before we diving into what integration test is. 
Let's determin why we need it.

> they ensure that modules which work well in isolation, also play well together.

Integration tests typically focus on a small number of modules and test their interactions.
So we may know what is integration test is from it.

> Intergration puts a small number of modules together to ensure they work well.
### e2e test
e2e(end to end) testing, where we test the whole application together, and test it as a user would — essentially automating whatever the user does.
So the E2E test should just check that the glue binding all units works.

But...
> relying primarily on end-to-end tests is a bad idea

and if you know testing pyramid, you could understand that easily.
## Visual Test
while
### snapshot
### screenshot


