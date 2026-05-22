Markdown Live Editor that supports:

- Katex and custom latex macros
- Exports slides in html and pdf format
- html/Javascript imports (dynamic, animations etc.)
- colors, font decorations with custom html tags
- image imports from local folders
- several theorem environments
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
  ## New section
  Large centered text
  ```
- `thanks`: Thanks slide  
  ```markdown
  thanks
  ---
  ## Thank You!
  - Q&A
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
  ## References
  - [1] Author, Title
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

## Inline Tags (you can also add your own)

### Color/Style
- `<r>`: red text  
  Ex: `<r>warning</r>` → <span style="color:#D15237">warning</span>
- `<rb>`: bold red  
  Ex: `<rb>ERROR</rb>` → <b style="color:#D15237">ERROR</b>
- `<g>`: green  
  Ex: `<g>success</g>` → <span style="color:#718c00">success</span>
- `<gw>`: light green  
  Ex: `<gw>note</gw>` → <span style="color:#8FC680">note</span>
- `<gb>`: bold green  
  Ex: `<gb>OK</gb>` → <b style="color:#718c00">OK</b>
- `<pur>`: purple bold large  
  Ex: `<pur>Title</pur>` → <b style="color:#B186C3;font-size:1.6rem">Title</b>
- `<ref>`: salmon  
  Ex: `<ref>[1]</ref>` → <span style="color:#E9967A">[1]</span>
- `<i>`, `<em>`: red italic-like  
  Ex: `<i>emphasis</i>` → <span style="color:#D15237">emphasis</span>
- `<b>`, `<strong>`: green bold  
  Ex: `<b>bold</b>` → <b style="color:#718c00">bold</b>

