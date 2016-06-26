PerkeleScript
==========
![Finnish Flag](/assets/img/flag.png)  
PerkeleScript lets you write JavaScript in Finnish; Finally there is a way for Fins to code in their native language!
It is named after [perkele](https://en.wikipedia.org/wiki/Perkele), the sacred Finnish bad word.

See it in action in your broser
### Including PerkeleScript files in your HTML

- Include [perkelescript.js](dist/perkelescript.js) and [perkelescript.browser.js](dist/perkelescript.browser.js).
- Make sure your html is set to allow utf-8 characters (add `<meta charset="utf-8">` in the <head>).

FikaScript supports the `text/perkelescript` MIME type. Any script tag with that type will be compiled and run automatically:
```html
<script type="text/perkelescript">
  j (x < 5) {
    konsoli.log("moi!");
  } muu {
    konsoli.log("moi!");
  }
</script>
```

You can also specify a `src` for your script tags: 
```html
<script type="text/perkelescript" src="snaps.perkelejs"></script>
```

#### Optional

##### Convert from PerkeleScript to JavaScript:

```javascript
PerkeleScript.finnishToEnglish(code); // returns a string representing the translated code
```

##### Convert from JavaScript to PerkeleScript:

```javascript
PerkeleScript.englishToFinnish(code); // returns a string representing the translated code
```

### Missing/incorrect translations?
You can see the translations over [here](https://github.com/pushmatrix/fikascript/blob/gh-pages/dist/fikascript.js#L4). Feel free to submit a pull request!

###TO-DOs
- Syntax highlighting for unicode chars
- npm support for command line compiling
- Add more translations!!! (ex: Array.pop, push, etc...)
