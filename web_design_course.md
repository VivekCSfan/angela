# Web Design Course

This is content from `Angela Yu` course on `complete web development`

[TOC]

## What happens on a webpage

For the sake of simplicity, we can say a `server` is a `computer` that is **running 24/7**

And `client` is your `regular laptop/computer`

When you type say `google.com`  is your `browser` will send that message to your `ISP` and your `ISP` will send the message to a `DNS server` which is nothing but a **souped up phone book** 

In other words `DNS server` **will look for** `exact IP address` of `url` here `google.com` which you typed in `browser`

**Every single computer** that is connected on `internet` has an `IP address` 

You can check `ip address` of any website using website `nslookup.io` 

So if you go to `nslookup.io` and type `google.com` and see the `IP address` of `google.com`

Now, you can copy that `IP address` and **directly paste in your** `browser` and still go to `google.com`

## How do websites actually work?!

There are three **main file types** they are `html` , `css` and `javascript`

`html` is used for **content** 

`css` is used for **styling the content**

`js` is used for **adding functionality** to a `webpage`

## Introduction to html

### What are tags and elements

`tags` refers to `<h1>` or `<\h1>` or other similar `symbols`

**some** `tags` **do not have** `closing tags`

`element` is **tag** and **it's entire contents**

For example, **entire line below** is called as `element` 

```html
<h1>Hello world</h1>
```

Always use `tags` in **hierarchy**

For example, after `h1` tags use `h2` tags. **Do not ignore** `a level`

**Do not** go from `h1` to `h3` tags without using `h2` tags on your webpage.

## Adding a line break

This is done using `<br />` tag

```html
<br />
```



## Adding a horizontal line

This is done using `<hr />` tag

```html
<br />
```



## Comparing with finished code

Suppose you are **coding along** and your `output` is not matching with `finished code` of some tutorial, then you can use `diffchecker.com` and see **changes** in both the codes.

## Creating lists 

There are `unordered lists` and `ordered lists`

### Unordered lists

They are created using `<ul>` and </ul>  tags 

And **each item** is wrapped in `<li>` and `</li>` tags

```html
<ul>
	<li>Study web design</li>
	<li>Study golang</li>
</ul>
```



### Ordered lists

This also has same form as `unordered lists` but it is created using `ol` and `</ol>`

```html
<ol>
    <li>Mathematics</li>
    <li>Programming</li>
</ol>
```

## Nested listing

You can have one `list` inside **another list**

```html
<ol>
    <li>Mathematics</li>
    <li>Programming</li>
    <li>Nested unordered list
        <ul>
            <li>First</li>
            <li>Second</li>
            <li>Third</li>
        </ul>  
    </li>
    <li>Another item</li>
</ol>
```



## Anchor tags

## Displaying images

`alt` tag is **essential** for `user accesibility`

## Screen reader

If you want to **read** the `contents` of a `webpage` we need `screen reader`  there is a `google chrome extension` called `silktide screen reader`

## Directory structure

You can use `relative` or `absolute` **file paths**

If you use `absolute filepaths` then it is **very difficult** to transfer your files 

But if you use `relative filepaths` you can simply copy and paste `project directory` anywhere and **no links will be broken**

To refer to **one directory above** `current directory` use `..` 

```html
<a href="../index.html" >"Fun site"</a>
```

Here `index.html` is located **one directory above** in `hierarchy`

## Creating a link with an image

```html
<a href="../index.html" ><img src="../download.jpeg" alt="fun" /></a>
```

## HTML template

**Every webpage** must have certain `elements` which are **essential for the web browser** 

For example `doctype` to indicate **which version** of `html` we are using on our site.

```html
<!DOCTYPE html>
<html lang="en"
```

Every webpage must contain `head` and `body` 

Contents in `head` **cannot be seen by** `web user` but it is for `crawlers` and `browsers`

```html
<!DOCTYPE html>
<html lang="en"
      <head>
		<meta charset="UTF-8"
       </head>        
```

`metacharset` when set to `UTF-8` **ensures that** our `webpage` gets **rendered correctly** in `browser`

`title` also goes into `head` section

```html
<!DOCTYPE html>
<html lang="en"
      <head>
		<meta charset="UTF-8"
              <title>My webpage title</title>
       </head>   
```

`title` **gets displayed** on `top` of your `browser window`

`<html lang="en"` **must end with** `</html`

```html
<!DOCTYPE html>
<html lang="en"
      <head>
		<meta charset="UTF-8"
              <title>My webpage title</title>
       </head>
</html>
```

In `vscode` you can use `!` and `hit ENTER` to **automatically insert** this `template`

## Dimensions of your webpage in browser

This is determined by `viewport`

In `head` section, add the following lines to **display** at `full size` In other words, **no magnification** or **reduction**

```html
<!DOCTYPE html>
<html lang="en"
      <head>
		<meta charset="UTF-8"
        <title>My webpage title</title>
		<meta name="viewport" content="width=device-width, initial-scale=1.0">
       </head>
</html>
```

## Hosting your website on github for free

Go to `settings` then go to `pages` then click then change `branch` from `none` to `main`

Then click `save`

