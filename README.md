# LineScript ![](https://img.shields.io/github/stars/ntrupin/LineScript.svg) ![](https://img.shields.io/github/forks/ntrupin/LineScript.svg) ![](https://img.shields.io/github/license/ntrupin/LineScript.svg)

<img src="https://raw.githubusercontent.com/ntrupin/LineScript/master/images/E81C9271-1AFE-487E-BDB0-5958E02F0ADB.jpeg" width="100%" />

The open source markup language that complies into HTML at runtime, providing beautiful, easy syntax to create webpages.

Like it? Leave us a star, it will help attract more visitors and contributors! 

## Our Mission

Primarily, our mission at LineScript is to help beginners and experts alike make their first contribution, and any that follow, to open source, and to find their place in the vast community. To do so, we created clear-cut contribution guides and examples, created rich documentation, have formulated a welcoming community, and are always around ourselves to lend a helping hand.

Secondarily, our mission at LineScript is to provide a way to develop interfaces for the web that is cleaner and more user-friendly than HTML. That means we removed clumped code, ugly opening/closing tag combinations, and trying to squeeze attributes into tags. The LineScript compiler only allows for one tag to be on a line, and it must follow a strict grammar. This leads to more uniform code that is nicer to the developer.

## The Problem

Modern web development (HTML/CSS/JS), though wonderfully functional and powerful, could be quite ugly to look at, and hard to navigate and edit, once there was a few dozen lines of code. These pages did not look like good writing (bad for your personal image, and your portfolio) and could be quite hard to continue work on.

## Our Goals

- Provide a vocabulary similar to HTML
- Create a strict grammar to enforce clean code
- Maintain a simple, powerful syntax to provide maximum functionality with a minimal learning curve

## What is LineScript? 

LineScript is a compiled programming language that is written in statements broken up by line to represent the page structure. It is compiled into a valid HTML document at runtime using the LineCompiler, and can be used to create real webpages. 

The structure of the document is inspired by a combination of [Elm](https://elm-lang.org) and [Haskell](https://haskell.org), while the tag names are close alterations of HTML. This leads to extremely clean code that is familiar to anyone who has developed for the web, making LineScript the perfect beginner and expert language.

## Why LineScript?

We believe that you should use LineScript because it provides a crisp, clean alternative to boring old HTML. What could be done in HTML with this:

```html
<!doctype html>
<html>
<head>
    <title>Example Domain</title>
    <meta charset="utf-8" />
    <meta http-equiv="Content-type" content="text/html; charset=utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <style type="text/css">
    body {
        background-color: #f0f0f2;
        margin: 0;
        padding: 0;
        font-family: "Open Sans", "Helvetica Neue", Helvetica, Arial, sans-serif;
        
    }
    div {
        width: 600px;
        margin: 5em auto;
        padding: 50px;
        background-color: #fff;
        border-radius: 1em;
    }
    a:link, a:visited {
        color: #38488f;
        text-decoration: none;
    }
    @media (max-width: 700px) {
        body {
            background-color: #fff;
        }
        div {
            width: auto;
            margin: 0 auto;
            border-radius: 0;
            padding: 1em;
        }
    }
    </style>    
</head>
<body>
<div>
    <h1>Example Domain</h1>
    <p>This domain is established to be used for illustrative examples in documents. You may use this
    domain in examples without prior coordination or asking for permission.</p>
    <p><a href="http://www.iana.org/domains/example">More information...</a></p>
</div>
</body>
</html>
```

Can easily be written in LineScript like this:

```css
charset -> utf-8
meta -> viewport -> width=device-width, initial-scale=1
link -> stylesheet -> index.css
title -> Hello, World!
div
 h1 -> Example Domain
 p -> This domain is established to be used for illustrative examples in documents. You may use this domain in examples without prior coordination or asking for permission.
 a -> href='http://www.iana.org/domains/example' -> More information...
end -> div
```

Linked to this stylesheet:

```css
body {
  background-color: #f0f0f2;
  margin: 0;
  padding: 0;
  font-family: "Open Sans", "Helvetica Neue", Helvetica, Arial, sans-serif;      
}
div {
  width: 600px;
  margin: 5em auto;
  padding: 50px;
  background-color: #fff;
  border-radius: 1em;
}
a:link, a:visited {
  color: #38488f;
  text-decoration: none;
}
@media (max-width: 700px) {
  body {
    background-color: #fff;
  }
  div {
    width: auto;
    margin: 0 auto;
    border-radius: 0;
    padding: 1em;
  }
}
```

Using LineScript's Runtime Compiler, the LineScript example displays the same exact output as the HTML example... and the developer wrote half as much code! Also, the LineScript part looks so much neater, don't you think? Writing LineScript is much nicer than HTML, and it doesn't require as much effort to write. So, why LineScript? Because it is shorter, easier, and cleaner.

## CSS/JS Capabilities

For styling documents in LineScript, you can link to external style sheets (such as [Bootstrap](https://getbootstrap.com) or [Skeleton](https://getskeleton.com)), use inline CSS, or use your own custom style sheet. All function of CSS3 is allowed, and extensions such as WebKit are able to be used.

JavaScript can be embedded in LineScript to interact with storage, the parsed HTML, servers, and more. LineScript also includes the ability to use JavaScript libraries such as [jQuery](https://jquery.com).

However, LineScript does not support embedded style sheets or scripts. All CSS or JavaScript must be written inline or in a separate document.

## Usage

See DOCS.md.

## Contributing

See CONTRIBUTING.md
