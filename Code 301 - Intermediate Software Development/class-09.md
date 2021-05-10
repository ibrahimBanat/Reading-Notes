# Refactoring and the essence of essence of clean code

code refactoring is the process of restructuring existing computer code—changing the factoring—without changing its external behavior. Refactoring is intended to improve the design, structure, and/or implementation of the software (its non-functional attributes), while preserving its functionality

What is the essence of clean code?

1. What is the essence of clean code?

When code is clean, you should be able to sit in a comfortable couch, by the fire, with a good drink and dim lights to enjoy the code like you would enjoy your favorite novel.

> Clean code tells you a story that is captivating and easy to follow.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1605224627517/2EGoh4afq.png?auto=compress)

2. Clean code is simple.

Clean code is so simple that it does not make the author look smart. And yet, it is obvious that the code was written by someone who put effort in it.

Because simple is not easy.

> First, you make it work. Then, you make it right ~ Kent Beck.

3. Clean code is tested.

A corollary of the previous section is that you can’t write clean code without refactoring. And, to refactor successfully, you need automated tests to guarantee that behavior does not change. Therefore, you need tests to write clean code.

It does not matter how clean the code is today. If it has no tests, you can't refactor confidently. Therefore, the code will become unclean because code tends to get more convoluted and coupled over time.

> The natural tendency of code is not towards cleanness. It is the opposite. Counteracting this tendency requires explicit action.

4. Clean code does not repeat itself.

Clean code says everything once.

This does not mean that duplication is eliminated blindly. Clean code avoids premature abstractions and it knows that, if two identical pieces of code represent different knowledge, removing duplication introduces risk.

5. Clean code speaks about the problem, not the solution.

If a name in your code includes a “computerish” term (such as “DTO”), it is probably focusing on “how”.

Clean code focuses on “what”.

Clean code uses terms that focus on the problem domain, not on the specific solution on a computer.

And these terms are at the right level of abstraction. If a software module is in the domain layer, the code will use terms of the domain model. If a module is in the database layer, it will speak about databases.

> Clean code uses the right level of abstraction to talk about the problem being solved.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1605224936681/FGHGtghUB.png?auto=compress)

## Conclusion

The main reason for me is that code is read far more times than it is written. Therefore, it is inefficient to favor solutions that make writing fast at the expense of making reading slow.

Always consider the consequences of your actions. Do not take steps back in your journey towards clean code.

> The only way to go fast is to go well ~ Uncle Bob.
