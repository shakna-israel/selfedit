# selfedit

A seriously hacky editor for text.

---

## Good god man! What have you done!?

This is a way to abuse your browser into compiling HTML-ish documents, and their editor, into a single link.

For example, copy and paste (if you're feeling brave) this little payload into a new URL:

    data:text/html;base64,PGRpdiBpZD0iYyIgY29udGVudGVkaXRhYmxlPSIiPjxkaXY+PGRpdj48aDE+IEhlYWRpbmc8L2gxPjwvZGl2PjwvZGl2PjxkaXY+PGRpdj48bGk+IExpc3QgaXRlbTwvbGk+PC9kaXY+PC9kaXY+PGRpdj48ZGl2PjxsaT4gTGlzdCBpdGVtPC9saT48L2Rpdj48L2Rpdj48ZGl2IGNsYXNzPSJxdW90ZSI+Jmd0OyBUaGlzIGlzIGEgcXVvdGUgLSBTb21lIGlkaW90PC9kaXY+PGRpdj48ZGl2PjxwcmU+Jm5ic3A7Jm5ic3A7Jm5ic3A7IGRlZiBmb28oKTo8L3ByZT48L2Rpdj48L2Rpdj48ZGl2PjxkaXY+PHByZT4mbmJzcDsmbmJzcDsmbmJzcDsmbmJzcDsmbmJzcDsmbmJzcDsmbmJzcDsgcGFzczwvcHJlPjwvZGl2PjwvZGl2PjxkaXY+VGhpcyBpcyBzb21lIHRleHQuIE9vaCwgYSA8YSBocmVmPSJodHRwczovL2V4YW1wbGUuY29tIj5saW5rPC9hPiEgQW5kIHNvbWUgPHN0cm9uZz5ib2xkPC9zdHJvbmc+IGFuZCBzb21lIDxlbT5pdGFsaWM8L2VtPi48L2Rpdj48ZGl2PkhvdyBhYm91dCBzb21lIDx1PnVuZGVybGluZWQ8L3U+IGFuZCBzb21lIDxzPnN0cnVjazwvcz4gdGV4dD88L2Rpdj48ZGl2PjxkaXY+PHByZT48L3ByZT48L2Rpdj48L2Rpdj48L2Rpdj4KPGEgaWQ9InAiIGhyZWY9IiI+Q29weSBtZTwvYT4KPHNjcmlwdD4KCXZhciBjID0gZG9jdW1lbnQuZ2V0RWxlbWVudEJ5SWQoJ2MnKTsKCXZhciBwID0gZG9jdW1lbnQuZ2V0RWxlbWVudEJ5SWQoJ3AnKTsKCgl3aW5kb3cuYWRkRXZlbnRMaXN0ZW5lcignbG9hZCcsIGZ1bmN0aW9uKCkgewoJCWMuYWRkRXZlbnRMaXN0ZW5lcignaW5wdXQnLCBmdW5jdGlvbihldmVudCkgewoJCQlwLnRleHRDb250ZW50ID0gJyc7CgkJCXAuaHJlZiA9ICcnOwoKCQkJaWYoZXZlbnQuaW5wdXRUeXBlICE9ICdpbnNlcnRUZXh0JyAmJiBldmVudC5pbnB1dFR5cGUgIT0gJ2RlbGV0ZUNvbnRlbnRCYWNrd2FyZCcpIHsKCgkJCQl2YXIgY2hpbGRyZW4gPSBjLnF1ZXJ5U2VsZWN0b3JBbGwoJyo6bm90KGJyKTpub3QocHJlKScpOwoKCQkJCWZvcih2YXIgaSA9IDA7IGkgPCBjaGlsZHJlbi5sZW5ndGg7IGkrKykgewoJCQkJCS8vIFRpdGxlcwoJCQkJCWlmKGNoaWxkcmVuW2ldLnRleHRDb250ZW50WzBdID09ICcjJykgewoJCQkJCQljaGlsZHJlbltpXS5pbm5lckhUTUwgPSAnPGRpdj48aDE+JyArIGNoaWxkcmVuW2ldLnRleHRDb250ZW50LnNsaWNlKDEpICsgJzwvaDE+PC9kaXY+JzsKCQkJCQl9CgoJCQkJCS8vIExpc3QgaXRlbQoJCQkJCWlmKGNoaWxkcmVuW2ldLnRleHRDb250ZW50WzBdID09ICcrJykgewoJCQkJCQljaGlsZHJlbltpXS5pbm5lckhUTUwgPSAnPGRpdj48bGk+JyArIGNoaWxkcmVuW2ldLnRleHRDb250ZW50LnNsaWNlKDEpICsgJzwvbGk+PC9kaXY+JzsKCQkJCQl9CgoJCQkJCS8vIENvZGVibG9ja3MKCQkJCQlpZihjaGlsZHJlbltpXS50ZXh0Q29udGVudC5zbGljZSgwLCA0KS50cmltKCkgPT09ICIiKSB7CgkJCQkJCWNoaWxkcmVuW2ldLmlubmVySFRNTCA9ICc8ZGl2PjxwcmU+JyArIGNoaWxkcmVuW2ldLmlubmVyVGV4dCArICc8L3ByZT48L2Rpdj4nOwoJCQkJCX0KCgkJCQkJLy8gUXVvdGVzCgkJCQkJaWYoY2hpbGRyZW5baV0udGV4dENvbnRlbnRbMF0gPT0gJz4nKSB7CgkJCQkJCWNoaWxkcmVuW2ldLmNsYXNzTGlzdC5hZGQoJ3F1b3RlJyk7CgkJCQkJfSBlbHNlIHsKCQkJCQkJY2hpbGRyZW5baV0uY2xhc3NMaXN0LnJlbW92ZSgncXVvdGUnKTsKCQkJCQl9CgoJCQkJCS8vIExpbmtzCgkJCQkJbGlua3MgPSBjaGlsZHJlbltpXS50ZXh0Q29udGVudC5tYXRjaCgvXFsoW1x3XHNcZF0rKVxdXCgoKD86XC98aHR0cHM/OlwvXC8pW1x3XGQuLz89I10rKVwpLyk7CgkJCQkJaWYoISFsaW5rcyAmJiBsaW5rcy5sZW5ndGggPiAyKSB7CgkJCQkJCWNoaWxkcmVuW2ldLmlubmVySFRNTCA9IGNoaWxkcmVuW2ldLmlubmVySFRNTAoJCQkJCQkJLnJlcGxhY2UobGlua3NbMF0sICc8YSBocmVmPSInICsgbGlua3NbMl0gKyAnIj4nICsgbGlua3NbMV0gKyAnPC9hPicpOwoJCQkJCX0KCgkJCQkJLy8gQm9sZAoJCQkJCS8vIEJVRzogRG9lc24ndCBtYXRjaCBjb3JyZWN0bHkgb24gbXVsdGlwbGVzIGluIHNhbWUgcGFyYWdyYXBoLgoJCQkJCWJvbGQgPSBjaGlsZHJlbltpXS50ZXh0Q29udGVudC5tYXRjaCgvXCpcKiguKylcKlwqLyk7CgkJCQkJaWYoISFib2xkICYmIGJvbGQubGVuZ3RoID4gMSkgewoJCQkJCQljaGlsZHJlbltpXS5pbm5lckhUTUwgPSBjaGlsZHJlbltpXS5pbm5lckhUTUwKCQkJCQkJCS5yZXBsYWNlKGJvbGRbMF0sICI8c3Ryb25nPiIgKyBib2xkWzFdICsgIjwvc3Ryb25nPiIpOwoJCQkJCX0KCgkJCQkJLy8gSXRhbGljcwoJCQkJCS8vIEJVRzogRG9lc24ndCBtYXRjaCBjb3JyZWN0bHkgb24gbXVsdGlwbGVzIGluIHNhbWUgcGFyYWdyYXBoLgoJCQkJCWl0YWxpY3MgPSBjaGlsZHJlbltpXS50ZXh0Q29udGVudC5tYXRjaCgvXCooLispXCovKTsKCQkJCQlpZighIWl0YWxpY3MgJiYgaXRhbGljcy5sZW5ndGggPiAxKSB7CgkJCQkJCWNoaWxkcmVuW2ldLmlubmVySFRNTCA9IGNoaWxkcmVuW2ldLmlubmVySFRNTAoJCQkJCQkJLnJlcGxhY2UoaXRhbGljc1swXSwgIjxlbT4iICsgaXRhbGljc1sxXSArICI8L2VtPiIpOwoJCQkJCX0KCgkJCQkJLy8gVW5kZXJzY29yZQoJCQkJCS8vIEJVRzogRG9lc24ndCBtYXRjaCBjb3JyZWN0bHkgb24gbXVsdGlwbGVzIGluIHNhbWUgcGFyYWdyYXBoLgoJCQkJCXVuZGVyc2NvcmUgPSBjaGlsZHJlbltpXS50ZXh0Q29udGVudC5tYXRjaCgvXF8oLispXF8vKTsKCQkJCQlpZighIXVuZGVyc2NvcmUgJiYgdW5kZXJzY29yZS5sZW5ndGggPiAxKSB7CgkJCQkJCWNoaWxkcmVuW2ldLmlubmVySFRNTCA9IGNoaWxkcmVuW2ldLmlubmVySFRNTAoJCQkJCQkJLnJlcGxhY2UodW5kZXJzY29yZVswXSwgIjx1PiIgKyB1bmRlcnNjb3JlWzFdICsgIjwvdT4iKTsKCQkJCQl9CgoJCQkJCS8vIFN0cmlrZXRocm91Z2gKCQkJCQkvLyBCVUc6IERvZXNuJ3QgbWF0Y2ggY29ycmVjdGx5IG9uIG11bHRpcGxlcyBpbiBzYW1lIHBhcmFncmFwaC4KCQkJCQlzdHJpa2UgPSBjaGlsZHJlbltpXS50ZXh0Q29udGVudC5tYXRjaCgvXH4oLispXH4vKTsKCQkJCQlpZighIXN0cmlrZSAmJiBzdHJpa2UubGVuZ3RoID4gMSkgewoJCQkJCQljaGlsZHJlbltpXS5pbm5lckhUTUwgPSBjaGlsZHJlbltpXS5pbm5lckhUTUwKCQkJCQkJCS5yZXBsYWNlKHN0cmlrZVswXSwgIjxzPiIgKyBzdHJpa2VbMV0gKyAiPC9zPiIpOwoJCQkJCX0KCgkJCQkJLy8gVE9ETzogSW1hZ2UgTGlua3MKCQkJCX0KCQkJCXAudGV4dENvbnRlbnQgPSAnQ29weSBtZSc7CgkJCQlwLmhyZWYgPSAiZGF0YTp0ZXh0L2h0bWw7YmFzZTY0LCIgKyBidG9hKGMucGFyZW50RWxlbWVudC5pbm5lckhUTUwpOwoJCQl9CgkJfSwgZmFsc2UpOwoJfSk7Cjwvc2NyaXB0Pgo8c3R5bGU+CiNwIHsKICBkaXNwbGF5OiBibG9jazsKICBtYXJnaW46IDAgYXV0bzsKICBwYWRkaW5nOiAxLjVlbTsKICB0ZXh0LWFsaWduOiBjZW50ZXI7Cn0KCiNjIHsKICB3aWR0aDogODAlOwogIHBhZGRpbmc6IDFlbTsKICBtYXJnaW46IDAgYXV0bzsKICBib3gtc2hhZG93OiAwcHggMHB4IDVweCAwcHggcmdiYSgwLDAsMCwwLjc1KTsKICBib3JkZXItcmFkaXVzOiAwLjJlbTsKICBsaW5lLWhlaWdodDoxLjU7Zm9udC1zaXplOiAxZW07Cn0KCnByZSB7CiAgZm9udC1mYW1pbHk6Q29uc29sYXMsTW9uYWNvLEx1Y2lkYSBDb25zb2xlLExpYmVyYXRpb24gTW9ubyxEZWphVnUgU2FucyBNb25vLEJpdHN0cmVhbSBWZXJhIFNhbnMgTW9ubyxDb3VyaWVyIE5ldywgbW9ub3NwYWNlOwogIHBhZGRpbmctbGVmdDogMS41ZW07Cn0KCi5xdW90ZSB7CiAgcGFkZGluZy1sZWZ0OiAwLjVlbTsKICBib3JkZXItbGVmdDogNnB4IHNvbGlkICNjY2M7CiAgYmFja2dyb3VuZC1jb2xvcjogI2YxZjFmMTsKICAKfQo8L3N0eWxlPgo=

Now, when we say copy and paste into the new URL, that is _exactly_ what we mean.

For security reasons, clicking that link may or may not actually open a new tab with the editor in it. Or it might open a new tab but not parse correctly.

This also may not work on Firefox Mobile, because contenteditable is somewhat broken on it, at time of writing.

This also may not work on Chrome, because they have an arbitrary limit on the length of a URL.

That being said, the entire URL is the document and editor. It doesn't load any other resources. It's self-contained, and can be safely used offline.

You can confirm the source of the document by decoding the base64 to see how it works.

The file, `selfedit.html` is our "base". However, once you've written a document, you can copy paste the `Copy me` link to get a self-contained file.

---

## It supports markup?

You may have noticed in our example link above that there are styles.

A very small and incredibly hacky "parser" exists to convert a tiny subset of Markdown-like things.

+ Lines beginning with `#` get turned into titles.

+ Lines beginning with `>` get turned into quotes.

+ Lines beginning with 4 spaces get turned into code blocks.

+ Lines beginning with `+` get turned into list items.

+ Links can be created like: `[Some text](https://example.com)`.

+ Bold can be created like: `**bold text**`.

+ Italic can be created like: `*italic text*`.

+ Underlined can be created like: `_underlined text_`.

+ Strikethrough can be created like: `~mispelsldj text~`.

---

## Oh no! A hit a bug!

... Yep. There's lots. I'll be somewhat interested in fixing them, but a lot of them are hard to reproduce. You're going to have to help me out by telling me exactly what you did to break it. I made this for fun. I won't be putting in a lot of effort.

And others are well known, like most of the bold/italic/underline/strikethrough stuff being somewhat broken.

---

## More Support!

I want it to support X feature!

_Shrug_. I might want it too. But... If you can send me a patch/pull request, I'd be more interested in helping you. But if I don't want it, too bad. This is a for-fun editor. _It isn't in any way shape or form appropriate for any purpose._ You get what it says on the tin.

---

## Speaking of support, can I pay you to work on this?

No.

### Can I, pretty please, pay you to work on this?

No. I hate JavaScript with an absolute passion. And this is a dumb idea.

If you really want something somewhat like this, then look into [TiddlyWiki](https://tiddlywiki.com/) and similar projects.

---

## I emailed my link and it disappeared!

Yep. Lots of email providers strip data URIs. Because they're dangerous. Which is why you shouldn't be touching this thing with a six foot pole.

---

## Can I inspect the contents of a link like this?

Sure. The basic format is:

    data:text/html;base64,$PAYLOAD

If you cut the `$PAYLOAD` out of the string, you can then put it into any base64 decoder and see the contents of the file. If anything looks obfuscated, run for the hills.

Understanding what you're copy and pasting is on you. I think I've said it before, but let me say it again: _This is not a safe thing to do!_

---

## License

So... You want to integrate or hack together something based atop this code?

Sure. You can do that, if you're insane.

Just be sure to read the `LICENSE` file very carefully, and agree to all its terms. It is _not_ a license you have read before.

Pay special attention to clauses 4 & 5, and consider how you will fulfill them in your role as maintainer.
