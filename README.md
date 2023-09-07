# MarkdownToHTML
This program was made to study rust with a hands-on approach rather than a textbook approach.
The main function defines two types of data structures; a Markdown structure and an HTML structure.
The Markdown structure has a path to the .md file, the name of the .md file (not including the .md, which is assumed) and new() contents.

From there, the user can run `let html: HTML = HTML::from_markdown(md_file);` which will convert the md file into an HTML string.
This can then be written to a file, using `html.to_file();`

# Planned Changes, Current Status, etc.
This program is in beta, as the `HTML::from_markdown(md)` does not have much functionality.
Finished functionality:
1. Headers
2. Ordered lists
3. Unordered lists

Planned functionality (in order of when it will be finished):
1. List tabs
2. Horizontal lines
3. Word formatting:
   - Bold
   - Italics
   - Strikethrough
   - Highlighted
5. Tasks
6. Comments
7. Codeblocks
8. Tables

# Future potentials
If this project goes far enough, I plan to look into making this into an API.
This API would read from my computer, and return an HTML file.
This would allow me to write markdown files for a static website and have them be dynamically converted to HTML when requested.
I also hope to use the GitHub Pages service so anyone can access the website without hosting it on my own server.

# Technologies used:
- Rust
- Markdown
- HTML
- Regex
