# automatr
A cool automation tool.
## Getting Started
Run ```npm i -g automatr``` in your terminal to install automatr.
In your project, create a file called ```autolist.json```, this is where all of your automation tasks will live.

Example ```autolist.json```

```json
{
  "compile": ["tsc index.ts", "tsc ./files/tests.ts"],
  "publish": ["git add .", "git commit", "git push"]
}
```

Now, if you run ```automatr compile``` it runs ```tsc index.ts``` and ```tsc ./files/tests/ts```. Same for ```publish```

You can create as many tasks as you want.
