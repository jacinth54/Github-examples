# markdown examples

- [unordered lists](#unordered-lists)
- ordered lists
- text formatting
- code
- tables
- blockquotes
- [links](#links)
- images
- autolinks
- lists

## Unordered lists

We can create unordered lists in markdown using hypens.

https://github.github.com/gfm/

- foo
- foo
+ bar

## ordered lists

1. foo
2. bar.
3. foo
3. foo
3) baz

## Text Formatting

*italics*
_italics_
**bold**
__bold__
~~strike~~

## Code

### Inline Code

You can print to terminal using the `puts "hello world"` command

### multiline Code


#### Without highlighting

```
def hello_world
    puts "Hello World"
end
```



#### with highlighting
```rb
def hello_world
    puts "Hello World"
end
```

### Tables

|foo|bar|
|---|---|
|baz|bim|

Cells in one column don’t need to match length, though it’s easier to read if they are. Likewise, use of leading and trailing pipes may be inconsistent:

| abc | defghi |
:-: | -----------:
bar | baz

| abc | def |
| --- | --- |
| bar |
| bar | baz | boo |

## Blackquote

> This is a block quote
> # This is a larger block quote

## Links

[test page](./test.md)

[GitHub website](https://github.com)

## Tasklist
- [ ] Item 1
- [x] Item 2