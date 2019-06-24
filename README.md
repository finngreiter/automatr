# automatr
A cool automation tool.
## Tutorial
To install, type ```npm i -g automatr``` into your terminal.

In your project directory, create a file called ```autolist.json```.

The ```autolist.json``` file is where your tasks will live.
Tasks are lists of terminal commands that get executed one by one.

### Making your first task
An example of a task is compiling a bunch of typescript files into javascript files. Heres an example project:

```
project_directory
-----autolist.json
-----index.ts
-----class.ts
```

And inside our ```autolist.json``` we create a task called ```compile```:

```json
{
  "compile": []
}
```

Inside the ```compile``` array, we add our terminal commands:

```json
{
  "compile": ["tsc index.ts", "tsc class.ts"]
}
```

To run the task, type ```automatr compile```.

You can create as many tasks as you want.
