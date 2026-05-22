Markdown Live Editor that supports:

- Katex and custom latex macros
- Export in html and pdf format
- html/Javascript imports (dynamic, animations etc.)
- colors, font decorations with custom html tags
- image imports from local folders
- several theorem and box environments
- several side types (references, contents etc.)

[Demo](http://barmpalias.net/share/md_slides/)

Based on the [cli version](https://github.com/bob7/md_slides)

<img src="Editor_screenshot.png" width="800" />

## Slide Types
Start slide with keyword + `---`

- `center`: Centered dark slide  
  ```markdown
  center
  ---
  ```
- `thanks`: Thanks slide  
  ```markdown
  thanks
  ---
  ```
- `iframe`: Include HTML (dark flex)  
  ```markdown
  iframe
  ---
  <iframe src="demo.html"></iframe>
  ```
- `frozen`: No page number  
  ```markdown
  frozen
  ---
  ```
- `references`: References list  
  ```markdown
  references
  ---
  ```

## Environment Blocks

### Theorems & Definitions (you can also add your own)
- `<thm>`: Theorem block  
  ```markdown
  <thm>
  Pythagoras: \(a^2 + b^2 = c^2\)
  </thm>
  ```
- `<thmc>`: Inline Theorem.  
  Ex: `<thmc> E=mc² </thmc>` → **Theorem.** E=mc²
- `<prop>`, `<propc>`: Proposition
- `<defi>`, `<defic>`: Definition
- `<fact>`, `<factc>`: Fact
- `<ex>`, `<exc>`: Example

### Questions
- `<quest>`: Question block (red label)  
  ```markdown
  <quest>
  Is P=NP?
  </quest>
  ```
- `<questc>`: Inline Question. 
- `<questce>`: Compact question block

### Box
- `<box>`: Light background box  
  ```markdown
  <box>
  Key point here
  </box>
  ```

## Inline Tags 

### Color/Style
- `<r>`: red text. Ex: `<r>warning</r>`.
- `<rb>`: bold red. Ex: `<rb>ERROR</rb>`
- `<g>`: green. Ex: `<g>success</g>` 
- `<gw>`: light green. Ex: `<gw>note</gw>` 
- `<gb>`: bold green. Ex: `<gb>OK</gb>` 
- `<pur>`: purple bold large. Ex: `<pur>Title</pur>` 
- `<ref>`: salmon. Ex: `<ref>[1]</ref>` 
- `<i>`, `<em>`: red italic-like. Ex: `<i>emphasis</i>` 
- `<b>`, `<strong>`: green bold. Ex: `<b>bold</b>` 
