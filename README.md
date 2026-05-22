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

## Import image
```markdown
![](./img/shuffle/3.png)
  ```


## Environment Blocks

### Theorems & Definitions

  ```markdown
  <thm>
  Pythagoras: \(a^2 + b^2 = c^2\)
  </thm>
  ```

- `<thm>`: Theorem block  
- `<thmc>`: Inline Theorem
- `<prop>`, `<propc>`: Proposition
- `<defi>`, `<defic>`: Definition
- `<fact>`, `<factc>`: Fact
- `<ex>`, `<exc>`: Example

### Questions
  ```markdown
  <quest>
  Is P=NP?
  </quest>
  ```
- `<quest>`: Question block (red label)  
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

  ```markdown
  <r>warning</r>
  ```

### Color/Style
- `<r>`: red text
- `<rb>`: bold red
- `<g>`: green
- `<gw>`: light green
- `<gb>`: bold green
- `<pur>`: purple bold large
- `<ref>`: salmon
- `<i>`, `<em>`: red italic-like
- `<b>`, `<strong>`: green bold

