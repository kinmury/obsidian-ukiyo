<h1 align=center>Features</h1>

## Centered Callouts

As you can probably guess by the heading, these callouts have their content centered by default. You don't need to do anything, the CSS got you covered. You just write whatever you want: Embeded notes, images, PDF, and it will be centered when you go to Preview View.

The only thing you need to do when you want to use these callouts is to put `-c` in front of one of the base classes of callouts. These classes are:

- `note-c`
- `abstract-c` / `summary-c` / `tldr-c`
- `info-c`
- `todo-c`
- `tip-c` / `hint-c` / `important-c`
- `success-c` / `check-c` / `done-c`
- `question-c` / `help-c` / `faq-c`
- `warning-c` / `caution-c` / `attention-c`
- `failure-c` / `missing-c`
- `danger-c` / `error-c`
- `bug-c`
- `example-c`
- `quote-c`

## Dataview Container and Items

There are two special callouts introduced with these theme:

- `> [!dv-container]` - As you can tell by the name, it's the *container* that will store the dataview queries that you make. But you can't just put the codeblock as it is, you need to put it inside a `dv-item`.
- `> [!dv-item]` - It's the dataview query it self. You should use one `dv-item` callout for each dataview query that you make, so it can flex properly inside the `dv-container`.

The reason why I created these callouts it's because, sometimes, tend to use some notes as *dashboards*. So I use a number of dataview queries. So, in order to have a more functional and easy to read dashboard, I design the previously mentioned callouts.

!!!	tip
	Instead of writing the `>` by hand, select all the dataview codeblock and use `CTRL+P` to open the **Command Panel**. Then, search for the `Insert Callout` command. This way, you only need to write the `dv-{type}` accordingly. I would suggest to bind a shortcut, since it's useful even for small and ordinary callouts.

## Callout Figures

There are times that I need to put a description to a centered image. Usually I would use `HTML` for this sort of things, but now that there are callouts, I use one of the following callouts:

- `> [!img-left]` - The elements inside the callout are centered on the inside of the callout, but the callout itself is located at the left side of the note.
- `> [!img-center]` - The elements inside the callout are centered on the inside of the callout and the callout itself is localted at the center of the note.
- `> [!img-right]` - The elements inside the callout are centered on the inside of the callout, but the callout itself is located at the right side of the note.

This way, I can use images, graphs, formulas, mermaids, and other things without any problem at all, creating more appealing and easy to understand notes. And also helps you develop a good looking essay.

## Pop Ups

If you used the **Golden Book** theme, you know what this is about, but instead of using the `<aside>`s, we'll use the callouts. For the folks that don't know what I'm talking about, these are the *Pop Ups*. Little squares located at the left side of your note. Inside those squared remains hidden information that you had written beforehand, and this information won't be shown unless you hover over said square. There are different types of *Pup Ups*:

- `> [!pu]` - The "by default" pop up, also know as *Note*
- `> [!pu-info]` - *Information*
- `> [!pu-imp]` - *Important*
- `> [!pu-quest]` - *Question*
- `> [!pu-check]` - *Check* / *Correct*
- `> [!pu-fail]` - *Fail* / *Incorrect*

There are two main improvements compared to the first version, the `<aside>` one:

1. **You can write whatever you want** - Since `<aside>` is a `HTML` element, you have to follow it's rules so that the information you use can be formatted correctly. For instance, if you want to write a **bold** text, you need to use `<b>bold</b>`, you want to use italic? `<i>italic</i>`. Also it made more complicated to insert images, tables, links, formulas among other things. Now, since we use callouts, these ain't gonna be an issue anymore.
2. **The animation is better, but not perfect** - Even though the transition of the *Pop Ups* are way better than the `<aside>`s one, it isn't perfect. Once you hover over the square, you shouldn't put the mouse on the left side of the pop up. If you do this, it will "glitch" and won't go back to its square form. I assure you it won't break anything, even if you do what I said, you only need to move the mouse away from it's path, and the transition will end accordingly.
	-  I don't know how I could "fix" this, since I only use CSS and I still have a lot to learn. If I manage to fix this issue, I will update it. But until them, this will be a constant issue. But I personally don't mind, since it only happens when the mouse is placed on the wrong side.

## Bookshelf

This feature it's inspired by the **Minimal Theme** made by *Kepano*. This feature on his theme is called `Cards`. But I can assure you my version is much more simplistic, so if you end up liking it, I really recommend you to go and check his theme. This feature is much more elaborate on this theme and some characteristics are only present on his theme, since I don't need it or it's way too much for what I need.

These feature is what you call a **CSS Class**, and for you to use it you need to put the following line somewhere on your frontmatter:

```yaml
---
cssClass: "dv-books"
---
```

This will enable the CSS code that make this feature work. If you have write this right away without much stuff on your note, you may see that nothing has change. The only thing that should change, are the dataview queries/tables.

This works for any dataview query, but its purpose is to create a table with all the books that you have search for on your query.

There are 2 things that needs to be considered when using this feature:

1. **Book Note** - You need to have a photo on the frontmatter, either the name of the image that you have on your Vault, or a link to an image on the internet. Both methods work.
2. **Dataview Query** - When you create the dataview query, you need to pay attention to the order of the table that you are creating. See the next example:

````
```dataview
TABLE WITHOUT ID

	embed(link(photo)),
	book-title,
	book-author,
	book-description

FROM "folder"

WHERE contains(tags, "book") = true
```
````

In this first example, it's assumed that you have this `YAML` on the *book note*:

```yaml
---
photo: "name-of-the-img-cover"
book-title: "Title"
book-author: "Author"
book-description: "Description"
---
```

In case that you use a link instead of a local note, you need to use the next code instead:

````
```dataview
TABLE WITHOUT ID

	photo,
	book-title,
	book-author,
	book-description

FROM "folder"

WHERE contains(tags, "book") = true
```
````

And the next `YAML` on the *book note*:

```yaml
---
photo: "![](url-of-the-img-cover)"
book-title: "Title"
book-author: "Author"
book-description: "Description"
---
```

## No Width

This is another **CSS Class** and its purpose is simple: Turn of the *Readable Line Length* of the note that it's being used. This class comes handy when combined with the `dv-books` or `dv-container` / `dv-item` combination.

When you want to use more than one **CSS Class**, you need to use an array. In `YAML` there are two ways of doing this and both ways will work, so it's a matter of preference.

```yaml
---
cssClass: ["css-class-1", "css-class-2"]
---
```


```yaml
---
cssClass:
- "css-class-1"
- "css-class-2"
---
```