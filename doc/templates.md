Templates
=========

* [Letter](#letter)
* [Invoice](#invoice)
* [Report](#report)
* [Slide deck](#slide-deck)


## Letter

The "Letter" template helps you write (formal) letters, usually to print and
send my mail.

### YAML Front-Matter

```yaml
---
date:
location:
addressFrom:
  name:
  street:
  zipCode:
  city:
addressTo:
  name:
  street:
  zipCode:
  city:
signature:
---
```

## Invoice

The "Invoice" template helps you write invoices.

### YAML Front-Matter

```yaml
---
reference:
date:
amount:
companyAddress:
  name:
  street:
  zipCode:
  city:
  country:
  businessID:
customerAddress:
  name:
  street:
  zipCode:
  city:
  country:
  businessID:
---
```

## Report

The "Report" template helps you write reports.

### YAML Front-Matter

```yaml
---
company:
  name:
  logo_url:
project:
reporter:
date:
location:
reference:
version:
---
```

## Slide deck

The "Slide deck" template helps you write awesome
[Reveal.js](https://github.com/hakimel/reveal.js)-based slides. In your Markdown
content, use a separator `---` (3 dashes) to split your content into different
**sections** (horizontally, like regular slide decks).

Thanks to Reveal.js, it is also possible to group slides into **sub-sections**
that are displayed vertically. Use `----` (4 dashes) to create sub-sections.

**Example:**

```markdown
Slide 1.0

---

Slide 2.0

----

Slide 2.1

----

Slide 2.2

---

Slide 3.0

----

Slide 3.1
```


### YAML Front-Matter

```
---
transition: zoom # None, Fade, Slide, Convex, Concave, Zoom
---
```

### Fragments

[Fragments](https://github.com/hakimel/reveal.js#fragments) are used to
highlight individual elements on a slide. You can use the `{fragment}` special
notation below any sentence or paragraph, and it will become a fragment.

``` markdown
---
transition: default
---

# Key metrics are:

* Fragment 1
{fragment}

* Fragment 2
{fragment}

* Fragment 3
{fragment}
```

### Style

#### Images

It is possible to hide the border of an image by using the `{no-border}` special
notation below the image:

```markdown
![](https://example.org/foobar.png)
{no-border}
```

#### Lists

It is possible to hide the bullets of a list by using the `{no-bullet}` special
notation:

```markdown
Isaac Asimov's "Three Laws of Robotics":

* A robot may not injure a human being or, through inaction, allow a human being
  to come to harm;
* A robot must obey orders given it by human beings except where such orders
  would conflict with the First Law;
* A robot must protect its own existence as long as such protection does not
  conflict with the First or Second Law.
{no-bullet}
```

#### Paragraphs

You can choose the paragraph alignment using the following special notations
on paragraphs (default being centered):

* `{left}`
* `{right}`
* `{justify}`


---
Back to: [Writing Monod documents](writing.md)
