<h1 align=center>Ukiyo</h1>

<p align=center>Welcome to <b>Ukiyo</b>, an Obsidian theme which main focus is to ease your eyes while using this amazin app, reducing the unnecessary empty spaces from UI elements so that you can have more room for the important stuff: <i>your notes</i>.</p>

## Galery

![](https://raw.githubusercontent.com/kinmury/obsidian-ukiyo/main/Showcase.png)
![](https://github.com/kinmury/obsidian-ukiyo/blob/main/imgs/Ukiyo_Default.png)
![](https://github.com/kinmury/obsidian-ukiyo/blob/main/imgs/Ukiyo_Deep.png)
![](https://github.com/kinmury/obsidian-ukiyo/blob/main/imgs/Ukiyo_Light.png)
![](https://github.com/kinmury/obsidian-ukiyo/blob/main/imgs/Ukiyo_GC.png)
![](https://github.com/kinmury/obsidian-ukiyo/blob/main/imgs/Ukiyo_GCD.png)
![](https://github.com/kinmury/obsidian-ukiyo/blob/main/imgs/Ukiyo_GC-Light.png)
![](https://github.com/kinmury/obsidian-ukiyo/blob/main/imgs/Ukiyo_GB.png)
![](https://github.com/kinmury/obsidian-ukiyo/blob/main/imgs/Ukiyo_ALCH.png)
![](https://github.com/kinmury/obsidian-ukiyo/blob/main/imgs/Ukiyo_ALCH-T.png)
![](https://github.com/kinmury/obsidian-ukiyo/blob/main/imgs/Ukiyo_ALCH-L.png)
![](https://github.com/kinmury/obsidian-ukiyo/blob/main/imgs/Ukiyo-ALCH-L-T.png)
![](https://github.com/kinmury/obsidian-ukiyo/blob/main/imgs/Ukiyo_RS.png)


# Utils

> Here is the list of all the utils that the theme provides, and by "utils" I mean all the Style Settings (`SS` for short) that the theme provide, along with all the CSS-Classes, Callouts, Tasks Icons, and all the CSS tools that I find useful.
> 
> There isn't a lot of utils for now, since I'm done with the update, not talking about all the new implementation that I want to add, but over time it will grow

- **Style Settings**
	- *General Settings*
		- <ins>Color Scheme</ins> - Lets you choose between the available color schemes that come with the theme: Golden Coffee, Golden Book, Alchemy and Rose Shadow.
	- *Color Schemes Specifics* - `in-progress` - Lets you change the properties of some of the elements like bold, italics, highlight and the font family. Said changes are applied to that color-scheme **and** used mode (dark and light) independently.
	- *UI - Visibility* - Choose which elements to hide and how to hide them
		- <ins>Side Dock Ribbon</ins>
	- *Modes* - Depending on the Color scheme, you can apply a mode to it:
		- <ins>Ukiyo Default</ins>
			- `Deep Dive` - Changes the default dark color scheme into one a little more darker one
		- <ins>Golden Coffee</ins>
			- `Dark Coffee` - For those who like dark coffee ;P
		- <ins>Alchemy</ins> 
			- `Enable texture` - By default, both dark and light mode won't have the "textures" the original Alchemy theme had, but you can bring it back by enabling this setting
		- <ins>Common Modes</ins> - These modes are common for all color schemes. For now there is just one:
			- `Smooth UI` - Make the UI smoother (yup, *shockingly unexpected*, I know XD)
- **Callouts** - There are a couple of custom callouts that you can use with this theme:
	- *`![<type>|center-title]`* - Using said "modifier" you can center the title
	- *`![<type>|center-cont]`* - Using said "modifier" you can center the content of the callout. You can stack modifiers by using a space in between the modifiers.
	- *`![cont]/![container]`* && *`![col]/![column]`* - Inside the `![cont]` callout, you can but as much `![col]` callouts as you want. This will let you create a custom kanban with any content that you may see fit. An good example would be using these "kanban-like-callouts" and the Dataview plugin to create a dynamic kanban query with notes that represent tasks.
	- *`![fig]/![figure]`* - Just like the LaTeX figures, all the content will be centered, so that you can put captions more easily below your images.
	- *`![clear-table]`* - The only content that should be inside this callout is a unique table. Said table won't have **any** CSS applied to it, so its just a clean table.
	- *`![index-table]`* - Same as the previous callout, but the thing is that the first row and the first column have the same distinctive background, so that you can create schedules, for example.
- **CSS Classes**
	- *full-width* - The note will expand as much as it can, as if the `readable line lenght` settings was disabled
	- *center-headings* - All headings will be centered
	- *DV_tasks* - Changes you Dataview tables into small blocks
- **Tasks/Checkboxes** - `TBD`

# Plugins

> Here are all the plugins that this theme has change to a large extends, not all plugins will be listed, since some of them aren't change to a degree that is worth mentioning.
> 
> The isn't a lot of plugins here, and I'm not sure if it will grow, since I'm comfortable with only a few plugins, but if there is a Feature Request about some plugin, I'll try my best to adapt it to the theme and add it here.

- **Kanban**
- **Editor Syntax Highlight** - `TBD`
- **Dataview**
- **Calendar**
