# Neat code block snippet

This snippet makes your Obsidian.md code blocks look a little fancier

![image](https://user-images.githubusercontent.com/92980051/189524728-183195dd-d146-44e1-a850-a0cada8d9cf0.png)

### How to install

1. Download the files (Code -> Download ZIP)
2. Open your Obsidian.md vault in explorer
3. Copy and paste the .obsidian folder in it
4. Go to: Obsidian app -> Settings -> Appearance -> CSS Snippets
5. Turn on "Neat code blocks"
6. (optional) copy and paste the 'Showcase.md' file to your vault too

### How to add my language?

1. Go to: Obsidian app -> Settings -> Appearance -> CSS Snippets
2. Open in explorer
3. Open the Neat code blocks.css
4. In the `:root { ... }` add:

```css
	/* I recommend copying the lang's logo color to here */
	--NAME-color: rgb(0, 0, 0);  /* or #ffffff. Left border color */
	--NAME-content: 'NAME';      /* displayed name */
```

5. Copy and paste this to the end of the file and change the `NAME`:
   
```css
pre>code.language-NAME {
	border-color: var(--NAME-color); /* change the name */
}

pre>code.language-NAME::after {
	content: var(--NAME-content);    /* change the name */
}
```

Might as well contribute after that
