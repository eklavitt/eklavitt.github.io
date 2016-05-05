---
title: "How Websites Work"
layout: post
date: 2016-05-05 12:30
tag:
- Client-Server Model
- Request-Response Cycle
- AJAX
blog: true
star: true
---

## Summary:

It was suggested that I take a few steps back in my web development path and really familiarize myself with how websites, and computers, work. I too often get ahead myself, assuming I know the basics, when in reality I don't. The relationship between the front-end and back-end is what makes displaying any web page possible, so why not explore how...

## What is the Front-end? What is the Back-end?

When I say "front-end," I'm really referring to the CLIENT. The client is a program that accesses a service in order to coherently display information to the user. One example is a web browser, which gathers the information to display a web page. 

But, where does the client get this information from? It would be unrealistic to assume that a web browser could store all of the information from every web page you want to view. SO, the browser (Client) has to ask for this information, which is stored on a very powerful specialized computer called a SERVER. 

Servers are the "back-end." As a basic definition, a server is a program or device that provides functionality for other programs or devices. They provide the resource or service for the client.

## Request-Response Cycle: 

Now I ponder, if I have one program with the information, and the other that wants the information, how does the exchange occur? The client simply requests the information, and the server responds with the information. This is known as the "Request-Response Cylce." This process generally has to be executed a number of times before any message can be properly displayed. 


The last thing to consider in this process is how the client and server find eachother. There are many servers throughout the world, as well as many clients, so they need a platform to find eachother. This is known as a NETWORK. The most familiar network is the internet, using addresses such as World Wide Web (www.---.com), that allow clients find the data to display the web page. 

This process is commonly call the CLIENT-SERVER Model.

## AJAX: Asynchronous JavaScript and XML

After understanding the client-server model, I wondered how this process of data exchange happens so smoothly, with such complex web pages. AJAX is the answer. It allows content to change dynamically without needing to reload the entire page (i.e multitasking!). Web pages can then communicate with servers in the background without interfering with the display and behavior of the existing page. 

This idea of "in the background" is the term ASYNCHRONOUS I/O (input and output). It won't block performance of other programs, rather allows them to process before the transmission is complete. 


## Conclusion:

Although it may seem simple, for a web page to display on your computer there needs to be a number of complex data exchanges between the Server containing the information and the Client requesting and receiving it over a network. Without this, we would all still be sending letters, using phone books, reading paperbacks and riding horses to work. 




<!-- ### Comum Elements
- [Basic formatting](#basic-formatting)
- [Headings](#headings)
- [Lists](#lists)
- [Paragraph Modifiers](#paragraph-modifiers)
- [Urls](#urls)
- [Horizontal Rule](#horizontal-rule)
- [Images](#images)
- [Code](#code)

---

## Basic formatting

This note **demonstrates** some of what [Markdown][1] is *capable of doing*.

And that's how to do it.

{% highlight html %}
This note **demonstrates** some of what [Markdown][some/link] is *capable of doing*.
{% endhighlight %}

---

## Headings

There are six levels of headings. They correspond with the six levels of HTML headings. You've probably noticed them already in the page. Each level down uses one more hash character. But we are using just 4 of them.

# Headings can be small

## Headings can be small

### Headings can be small

#### Headings can be small

{% highlight raw %}
# Heading
## Heading
### Heading
#### Heading
{% endhighlight %}

---

## Lists

### Ordered list

1. Item 1
2. A second item
3. Number 3

{% highlight raw %}
1. Item 1
2. A second item
3. Number 3
{% endhighlight %}

### Unordered list

* An item
* Another item
* Yet another item
* And there's more...

{% highlight raw %}
* An item
* Another item
* Yet another item
* And there's more...
{% endhighlight %}

---

## Paragraph modifiers

### Quote

> Here is a quote. What this is should be self explanatory. Quotes are automatically indented when they are used.

{% highlight raw %}
> Here is a quote. What this is should be self explanatory.
{% endhighlight raw %}

---

## URLs

URLs can be made in a handful of ways:

* A named link to [Mark It Down][3].
* Another named link to [Mark It Down](http://markitdown.net/)
* Sometimes you just want a URL like <http://markitdown.net/>.

{% highlight raw %}
* A named link to [MarkItDown][3].
* Another named link to [MarkItDown](http://markitdown.net/)
* Sometimes you just want a URL like <http://markitdown.net/>.
{% endhighlight %}

---

## Horizontal rule

A horizontal rule is a line that goes across the middle of the page.
It's sometimes handy for breaking things up.

{% highlight raw %}
---
{% endhighlight %}

---

## Images

Markdown can also contain images. I'll need to add something here sometime.

{% highlight raw %}
![Markdowm Image][/image/url]
{% endhighlight %}

![Markdowm Image][6]

*Figure Caption*?

{% highlight raw %}
![Markdowm Image][/image/url]
<figcaption class="caption">Photo by John Doe</figcaption>
{% endhighlight %}

![Markdowm Image][6]
<figcaption class="caption">Photo by John Doe</figcaption>

*Bigger Images*?

{% highlight raw %}
![Markdowm Image][/image/url]{: class="bigger-image" }
{% endhighlight %}

![Markdowm Image][6]{: class="bigger-image" }

---

## Code

A HTML Example:

{% highlight html %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
</head>
<body>
    <h1>Just a test</h1>
</body>
</html>
{% endhighlight %}

A CSS Example:

{% highlight css %}
pre {
    padding: 10px;
    font-size: .8em;
    white-space: pre;
}

pre, table {
    width: 100%;
}

code, pre, tt {
    font-family: Monaco, Consolas, Inconsolata, monospace, sans-serif;
    background: rgba(0,0,0,.05);
}
{% endhighlight %}

A JS Example:

{% highlight js %}
// Sticky Header
$(window).scroll(function() {

    if ($(window).scrollTop() > 900 && !$("body").hasClass('show-menu')) {
        $('#hamburguer__open').fadeOut('fast');
    } else if (!$("body").hasClass('show-menu')) {
        $('#hamburguer__open').fadeIn('fast');
    }

});
{% endhighlight %} -->

[1]: http://daringfireball.net/projects/markdown/
[2]: http://www.fileformat.info/info/unicode/char/2163/index.htm
[3]: http://www.markitdown.net/
[4]: http://daringfireball.net/projects/markdown/basics
[5]: http://daringfireball.net/projects/markdown/syntax
[6]: http://kune.fr/wp-content/uploads/2013/10/ghost-blog.jpg
