Hello once again 😁

I know I haven't been very active on the development of the theme, but I got a lot of work on my plate and didn't really have time to work properly on the theme to implement all the things that needed to be added or to fix and add the new features that where asked about.

Quick summary of what happened this past months: I've been customizing all the details that were left undone and adding new stuff as I was developing it in my not-quite-a-lot spare time. I have added a few fonts, added a new color scheme, fixed a few issues, added some animations here and there, and tried out some stuff regarding the UI appearance/"functionality". At the end... not only I had "kinda a big mess" of theme (cause all the stuff that I've been implementing) but also because of the fonts... The CSS file got big... 7 MB kind of big... so yeah... there's that...

This past weeks I got fed up with this aspect of the theme, since my main goal is to try to keep it as simple and elegant as possible, but also that you can add up whatever you want on top of it.... and there it hit me: _Style Settings_ and _Snippets_.

This isn't something new, and quite a few theme already relays on said functionalities in order to provide a better theme for themselves and all the users that like/want to use said theme. In my case, I really didn't think a lot of it, cause all the stuff that I use is quite simple... or at least that's what I've thought.

Ending the backstory I'll be talking about what I'll be doing (or at least trying... since my studies/work tend to get harder to finish/work on):
- [ ] **Clean Version** - On this branch (`dev`) you should find a `clean.css` version of the `soon-2-be-ukiyo` theme, were there is no color schemes or any fancy things (fonts and icons mostly) what so ever. This will be the base for everything that's coming forward.
- [ ] **Mobile Compatibility** - I've been procrastinating long enough the Mobile compatibility. It's time for me to also try and adapt my theme for the mobile users (I don't really use it on mobile, but I know that there are quite a few people that do, and I don't want to limit the theme for only _PC_ users).
- [ ] **Style Setting** - Instead of adding all the color schemes, I'll try to create all the settings necessary for me to implement said color schemes using these settings. So, instead of "hard-coding" all the color schemes, I'll create all the *Style Settings - Settings* witch all the configuration needed to get said color schemes on your local vault.
	- By doing this, not only I'll be reducing the size of the CSS file by not including all the Color Schemes that, more often than not, you'll end up not using, but also I'll be giving you the change to create your own color scheme (and share it with others if you want 😉)
	- Also, there will be two separate set of SS-settings:
		- [ ] *Dark Mode*
		- [ ] *Light Mode*
	- This way, you can customize each view to be exactly as you want it to be
- [ ] **Color Schemes Pres-sets** - Once the *Style-Settings Settings* are implemented and working correctly, I'll re-create all the Color Schemes that where present during the last Ukiyo version, the ones that where being developed during this month and, if I find the inspiration/time, a new one, but that's still in the air.
- [ ] **Snippets Gallery** - One of the things that tend to take quite a lot of space are the *text and icon-related fonts*. This past month I took it personally to configure the theme in order to show the fonts the way I want them, and with the font-weight that I wanted... but the CSS-file-size took **the** hit.
	- So, instead of loading the CSS file unnecessary, since not all users would like the font that I've chosen, I'll just create a bunch of snippets that you can add to the theme or any other, since it will act as a *separate and independent module*. This also goes for the icon icons.

I'll be publishing a `alpha/beta-version.css` file that you can get and try out the development of the theme. I don't want to forward it to the main branch since there is the official theme. Once it's finished I'll push it there so that everyone can enjoy it.

And, just to wrap this up, I just wanted to thank every single one of the users that have used/are using/will be using my theme (and for letting me know if something is broken or that could be improved 😉). I really hope that you like the direction the development of the theme is taking and, if by any chance, you feel like adding X feature would be great, I'll be glad to hear it on the issues sections 😁

Once again, thank you and have a beautiful day 😊