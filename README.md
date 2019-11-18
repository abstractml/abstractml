# AbstractML
*AbstractML: Abstract Markup Language*

![](https://img.shields.io/github/stars/ntrupin/abstractml.svg) ![](https://img.shields.io/github/forks/ntrupin/abstractml.svg)

### We're looking for someone to help maintain the project. If you would like to help, please open an issue.

An HTML abstraction focused on simplicity, providing beautiful, easy syntax to create webpages.

Like it? Leave us a star, it will help attract more visitors and contributors! 

Using AbstractML, you can write markup both more simple and more readable, providing a more straightforward way to design beautiful webpages!

In short, it allows you to replace this:

<img src="/docs/DBA72F07-A2FB-4B59-B26D-B96855CEFD68.jpeg" align="right" height="280px" hspace="30px" max-width="75%" vspace="30px">

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>Hello, world!</h1>
        <hr>
        <p>This is HTML</p>
    </body>   
</html>
```

with this

```CSS
h1 > Hello, world!
hr
p > This is AbstractML!
```

## Our Mission

Primarily, our mission at AbstractML is to help beginners and experts alike make their first contribution, and any that follow, to open source, and to find their place in the vast community. To do so, we created clear-cut contribution guides and examples, created rich documentation, have formulated a welcoming community, and are always around ourselves to lend a helping hand.

Secondarily, our mission at AbstractML is to provide a way to develop interfaces for the web that is cleaner and more user-friendly than HTML. That means we removed clumped code, ugly opening/closing tag combinations, and trying to squeeze attributes into tags. The AbstractML compiler only allows for one tag to be on a line, and it must follow a strict grammar. This leads to more uniform code that is nicer to the developer.

## The Problem

Modern web development (HTML/CSS/JS), though wonderfully functional and powerful, could be quite ugly to look at, and hard to navigate and edit, once there was a few dozen lines of code. These pages did not look like good writing (bad for your personal image, and your portfolio) and could be quite hard to continue work on.

## Our Goals

- Provide a vocabulary similar to HTML
- Create a strict grammar to enforce clean code
- Maintain a simple, powerful syntax to provide maximum functionality with a minimal learning curve

## What is AbstractML? 

AbstractML is a compiled language that is written in statements broken up by line to represent the page structure. It is compiled into a valid HTML document at runtime using the compiler, and can be used to create real webpages. 

The structure of the document is inspired by a combination of [Elm](https://elm-lang.org) and [Haskell](https://haskell.org), while the tag names are close alterations of HTML. This leads to extremely clean code that is familiar to anyone who has developed for the web, making AbstractML the perfect beginner and expert language.

## Why AbstractML?

We believe that you should use AbstractML because it provides a crisp, clean alternative to boring old HTML. What could be done in HTML with this:

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Example Domain</title>
        <meta charset="utf-8" />
        <meta http-equiv="Content-type" content="text/html; charset=utf-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1" />
        <link rel="stylesheet" href="index.css" />
    </head>
    <body>
        <div>
            <h1>Example Domain</h1>
            <p>This domain is for use in illustrative examples in documents. You may use this domain in literature without prior coordination or asking for permission.</p>
            <p><a href="http://www.iana.org/domains/example">More information...</a></p>
        </div>
    </body>
</html>
```

Can easily be written in AbstractML like this:

```css
title > Example Domain /
meta | charset="utf-8" /
meta | http-equiv="Content-type" content="text/html; charset=utf-8" /
meta | name="viewport" content="width=device-width, initial-scale=1" /
link | rel="stylesheet" href="index.css" /
div
    h1 > Example Domain /
    p > This domain is for use in illustrative examples in documents. You may use this domain in literature without prior coordination or asking for permission. /
    a | href='http://www.iana.org/domains/example' > More information... /
/ div
```

Both pages were linked to this stylesheet:

```css
body {
  background-color: #f0f0f2;
  margin: 0;
  padding: 0;
  font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", "Open Sans", "Helvetica Neue", Helvetica, Arial, sans-serif;
}

div {
  width: 600px;
  margin: 5em auto;
  padding: 2em;
  background-color: #fdfdff;
  border-radius: 0.5em;
  box-shadow: 2px 3px 7px 2px rgba(0, 0, 0, 0.02);
}

a:link,
a:visited {
  color: #38488f;
  text-decoration: none;
}

@media (max-width: 700px) {
  div {
    margin: 0 auto;
    width: auto;
  }
}
```

Using AbstractML's Runtime Compiler, the AbstractML example displays the same exact output as the HTML example... and the developer wrote nearly half as much code! Also, the AbstractML part looks so much neater, don't you think? Writing AbstractML is much nicer than HTML, and it doesn't require as much effort to write. So, why AbstractML? Because it is shorter, easier, and cleaner.

## CSS/JS Capabilities

For styling documents in AbstractML, you can link to external style sheets (such as [Bootstrap](https://getbootstrap.com) or [Skeleton](https://getskeleton.com)), use inline CSS, or use your own custom style sheet. All function of CSS3 is allowed, and extensions such as WebKit are able to be used.

JavaScript can be embedded in AbstractML to interact with storage, the parsed HTML, servers, and more. AbstractML also includes the ability to use JavaScript libraries such as [jQuery](https://jquery.com).

However, AbstractML does not support embedded style or script tags with code nested in them. All CSS or JavaScript must be written inline or in a separate document.

## Documentation

The documentation can be found [here](https://ntrupin.github.io/abstractml/).

## Contributing

See CONTRIBUTING.md
