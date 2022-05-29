# Regex

Regex is Regular expression, which you can use it to do string matching.

For example, there are a string and you need to find all of `OK` in it:
```
Understand? OK or NOT
```

That's will be easy, you can use string matching algorithm like BM, KMP or Sunday. But if I want to find all of the email addresses in the following paragraph?
```
My email is admin@example.com, and my girlfriend's email is gf@example.com, but why you display mine as admin#exmaple.com?
```

You need to find: `admin@example.com` and `gf@example.com`, but not should to find `admin#example.com`.

So the easy way is failure, and you need to write a state machine to solve the problem. But if I want to write an universal state machine to solve all problem, and we just give the machine two parameters: PROBLEM and INPUT. So the regex is the PROBLEM of it. In the email situation, it likes this:
```regexp
[^@ \t\r\n]+@[^@ \t\r\n]+\.[^@ \t\r\n]+
```

We suggest that you can learn from [regex101](https://regexlearn.com/learn/regex101), it's a good guide. And when using regex, try to find the existed at [iHateRegex](https://ihateregex.io/) first.

## Tools

* [Regexper](https://regexper.com/) - Regular Expression Visualization
* [Regex-Vis](https://regex-vis.com/) - Regex visualizer & editor
* [iHateRegex](https://ihateregex.io/) - Common regexs here
* [regexlearn.com](https://github.com/aykutkardas/regexlearn.com) - Learn RegEx step by step, from zero to advanced