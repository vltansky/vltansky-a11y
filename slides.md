---
# try also 'default' to start simple
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/9xxNZCJZ8bA/1920x1080
# apply any windi css classes to the current slide
class: "text-center"
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Leumi a11y 
  A11y basics for developers.
drawings:
  persist: false
# page transition
transition: slide-left
# use UnoCSS
css: unocss
---

# Digital Asakim A11y

<div class="text-center my-5">
  <img src="/imgs/a11y-exp.png" class="inline" />
</div>

##### “ a11y ” stands for “accessibility.” It is a numeronym, with 11 representing the count of letters between the letter a and the letter y. Other numeronyms you may be familiar with include: i18n (internationalization)

---

# Other abbreviation explanation

- W3C - World Wide Web Consortium (1994)
- WAI - Web Accessibility Initiative (1997) <br />
  by W3C & The White House
- WCAG - Web Content Accessibility Guidelines (December 2008)
- SR - Screen reader
- AT - Assistive technology - Any item, piece of equipment, or product system that is used to increase, maintain, or improve functional capabilities of individuals with disabilities

---

# WCAG

WCAG 2.0 guidelines are categorized into three levels of conformance: A (lowest), AA (mid range), and AAA (highest).

https://en.wikipedia.org/wiki/Web_Content_Accessibility_Guidelines#Version_2 <br/>
https://www.w3.org/TR/WCAG22 <br/>
https://www.w3c.org.il/guidelines_wcag_2-0 <br/>
https://uxdesign.cc/wcag-3-0-what-you-need-to-know-about-the-future-of-accessibility-standards-2e1f6374f2c7


---

# WCAG Perceivable

## נתפס

- Make all functionality available from a keyboard.
- Give users enough time to read and use content.
- Do not use content that causes seizures or physical reactions.
- Help users navigate and find content.
- Make it easier to use inputs other than keyboard.

---

# WCAG Operable

## ניתן להפעלה

- Make all functionality available from a keyboard.
- Give users enough time to read and use content.
- Do not use content that causes seizures or physical reactions.
- Help users navigate and find content.
- Make it easier to use inputs other than keyboard.

---

# WCAG 4 Principes

---

# WCAG Understandable

## ניתן להבנה

- Make text readable and understandable.
- Make content appear and operate in predictable ways.
- Help users avoid and correct mistakes.

---

# WCAG Robust

## יציב

- Maximize compatibility with current and future user tools.

---

# WCAG in law

By Law: https://www.w3.org/WAI/policies/

The Israeli accessibility regulations were amended in 2017 to require web accessibility in all services provided over the internet. Both private and public entities providing services online are required to apply Internet Accessibility Standard (Israel Standard 5668), which has adopted WCAG 2.0. The regulations apply to both websites, at AA level, and to applications and to digital documents uploaded after Oct 2017. Personal information – such as bank client’s statements – is to be made accessibly by 2022. Accessible websites and apps are required to include an accessibility statement.
<br/><br/>
Captions are required for time-based media (Level A) uploaded after 2017. However, only public authorities and large-scale private businesses have to provide them. In addition, lectures, conferences and similar events presented online, may offer a text document as alternative to online accommodations. Services provided or promoted through social media are required to use the accessibility features offered by the platforms. Websites which host third-party content have to provide accessibility options, such as alt text descriptions for images.
<br/><br/>
Small businesses may be granted an exemption, limited to 3 years. Exemptions may also be granted to any service, if the accommodations are technically impossible. The regulations are enforced both administratively, by the Commission on Equal Rights for Persons with Disabilities – a government agency – and through civil legal proceedings.

---

# How to use A11y software

Softwares:

- Jaws
- NVDA
- VoiceOver [keys](https://help.apple.com/voiceover/command-charts/)

https://www.tpgi.com/basic-screen-reader-commands-for-accessibility-testing/

Arrow keys - navigate
Tab key - jump to next focusable element (element should trigger smth, not just read)


---

# Semantic HTML5 and layout wai aria
<div class="text-center">
  <img src="/imgs/semantic-twit.jpg" class="inline h-[280px]" />
  <img src="/imgs/non-semantic.png" class="inline h-[280px]" />
</div>

https://www.semrush.com/blog/semantic-html5-guide/

---


# Focus

### `:focus` & `:focus-visible`

https://hidde.blog/focus-visible-more-than-keyboard/#:~:text=In%20other%20words%2C%20focus%20styles,to%20highlight%20it%20or%20not.

### Focus trap

https://appnest-demo.firebaseapp.com/focus-trap/

## Styling focus

https://tailwindcss.com/docs/hover-focus-and-other-states#hover-focus-and-active


### Autofocus



---

# TabIndex & ESlint

tabindex = 0 | -1 | 1,2,3...

🚫 Not accessible

  <img src="/imgs/a11y-eslint-onclick.png" class="inline h-[150px]" />

✅ Good

```jsx{all|2|3-4}
<div
  tabIndex={0}
  onKeyDown={(e)=>e.keyCode === 13 && alert('a')}
  onClick={()=>alert('a')}
  >
  test
</div>
```
* `onKeyPress` deprecated -  use `onKeyDown`,

---

# Buttons

Always prefer `<button>` over divs, spans etc. Button by default handles space and enter keypress.

- `<div role="button" />`
- `<button>` types = submit (default) | button | reset
- `<input type="button">`


```jsx{3|2-3|4}
<div 
  tabindex="0" 
  role="button" 
  aria-pressed="false"
  >
  Save
</div>
```

---

# Navigation

```html{all|1,10|2,9|3,5|4}
<nav aria-label="Main">
   <ul>
      <li>
        <a href="/about.xhtml">About</a>
      </li>
      <li><a href="/news.asp">News</a></li>
      <li><a href="/register.cfm">Register</a></li>
      […]
   </ul>
</nav>
```

or use aria:
```html
<div role="navigation" aria-label="Main">
  <!-- list of links to main website locations -->
</div>
```

## role=menu|menubar|menuitem are desktop menus
https://adrianroselli.com/2017/10/dont-use-aria-menu-roles-for-site-nav.html


---

# Dropdowns

https://adrianroselli.com/2020/03/stop-using-drop-down.html

---

# Images
### svg

```html
<svg>
  <title>Qr code</title>
</svg>
```

```html
<svg aria-label="Qr code">
  ...
</svg>
```
<br />

### img - use `alt`. If image not informative - leave empty alt. 

```html
<img src=".." alt="" />
```
<br />

### font icons

```html
<span class="fa-solid fa-envelope" aria-hidden="true"></span>
<span class="fa-solid fa-envelope" aria-label="explanation"></span>
```

---

# Hiding elements

- `aria-hidden="true"`
- `role="presentation"` same as `role="none"`

seem similar, but the intent behind each is different.

aria-hidden="true" will remove the entire element from the accessibility API.
role="presentation" and role="none" will remove the semantic meaning of an element while still exposing it and its content to assistive technology.

The HTML hidden attribute is present
The element or the element's ancestor is hidden with display: none
The element or the element's ancestor is hidden with visibility: hidden
In all three scenarios, the attribute is unnecessary to add because the element has already been removed from the accessibility tree. Visually hiding elements with display or visibility hides content from the screen and from assistive technologies.

Using aria-hidden="false" will not re-expose the element to assistive technology if any of its parents specify aria-hidden="true".

https://www.digitala11y.com/presentation-role/ (Example 4)
---

# Showing elements only for screen readers

```css
.sr-only {
  position: absolute;
width: 1px;
height: 1px;
padding: 0;
margin: -1px;
overflow: hidden;
clip: rect(0, 0, 0, 0);
white-space: nowrap;
border-width: 0;
}
```

* sr = screen reader

https://tailwindcss.com/docs/screen-readers


---

# Devtools

---

# aria-live region + aria busy
---
# Table structure + a bit about our Table component
---
# Error (role=“alert” + aria-describedby)
---
# Label -> for or wrap
---
# useId react + id should be unique
---
# Whisper + trigger cant be div!
---
# role=“slider” example
---
# tabpanel + accordions
---
# Checkbox
---
# Radio
---
# Input
---
# Autocomplete
---

https://github.com/alphagov/accessible-autocomplete
# Motion disabled
---

# Useful links

https://www.smashingmagazine.com/2021/03/complete-guide-accessible-front-end-components/
