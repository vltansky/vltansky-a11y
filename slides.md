---
# try also 'default' to start simple
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
# background: /imgs/a11y-bg.png
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

# 
<div class="bg-[url(/imgs/a11y-bg.png)] h-[100vh] w-full bg-contain fixed left-0 top-0" />
<div class="text-white bottom-8 absolute">“ a11y ” stands for “accessibility.” It is a numeronym, with 11 representing the count of letters between the letter a and the letter y. Other numeronyms you may be familiar with include: i18n (internationalization)</div>


---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# Other abbreviation explanation

- W3C - World Wide Web Consortium
- WAI - Web Accessibility Initiative <br />
  W3C Accessibility Initiative (expanding scope of accessibility standards to more than just web content)
- WCAG - Web Content Accessibility Guidelines
- SR - Screen reader
- AT - Assistive technology - Any item, piece of equipment, or product system that is used to increase, maintain, or improve functional capabilities of individuals with disabilities

<!--
* i18n,l10n
* AGWG has decided WCAG no longer stands for “Web Content Accessibility Guidelines”. It now stands for “	”. This change reflects the expanding scope of accessibility standards to more than just web content
-->
---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# WCAG

WCAG 2.0 guidelines are categorized into three levels of conformance: A (lowest), AA (mid range), and AAA (highest).

https://en.wikipedia.org/wiki/Web_Content_Accessibility_Guidelines#Version_2 <br/>
https://www.w3.org/TR/WCAG22 <br/>
https://www.w3c.org.il/guidelines_wcag_2-0 <br/>
https://uxdesign.cc/wcag-3-0-what-you-need-to-know-about-the-future-of-accessibility-standards-2e1f6374f2c7

<!--
* founded 1995
* WCAG 2.0, were published in December 2008


WCAG 3.0 isn’t supposed to finalize until 2023. Don’t be surprised if it gets pushed to an even later date, though.

WCAG 2.2 is at the Candidate Recommendation stage of the process, and we expect it to be finalized in early 2023. won’t change much.

WCAG 3.0 will not be backwards compatible with the WCAG 2 Series; but the 2 Series will not be deprecated by the 3 Series. Both will be parallel standards.

Once WCAG 3.0 is finalized AGWG plans on having more frequent updates. They have adopted an Agile approach to the standards. AGWG recognizes it’s far more difficult to future-proof the standards, especially with scope of the content going beyond the web.
-->

---
layout: center
class: "bg-[url(/imgs/bg.png)] bg-cover"
---
# WCAG 4 Principes

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# WCAG Perceivable

## נתפס

- Provide text alternatives for non-text content.
- Provide captions and other alternatives for multimedia.
- Create content that can be presented in different ways, including by assistive technologies, without losing meaning.
- Make it easier for users to see and hear content.
<!--
* 1 נתפס
    * 1.1 יש לספק חלופות טקסטואליות עבור תכנים לא טקסטואליים, כך שניתן יהיה להמירם לצורות אחרות להן זקוקים אנשים, כמו אותיות גדולות, ברייל, דיבור, סמלים או שפה פשוטה יותר.
    * 1.2 יש לספק חלופות עבור מדיה מבוססת-זמן.
    * 1.3 יש לבנות תכנים הניתנים להצגה בדרכים שונות (למשל outline פשוט יותר) ללא איבוד מידע או מבנה.
    * 1.4 יש להקל על המשתמשים לראות ולשמוע תכנים לרבות הפרדת חזית מרקע.
-->

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# WCAG Operable

## ניתן להפעלה

- Make all functionality available from a keyboard.
- Give users enough time to read and use content.
- Do not use content that causes seizures or physical reactions.
- Help users navigate and find content.
- Make it easier to use inputs other than keyboard.
<!--    
* 2 ניתן להפעלה
    * 2.1 יש לאפשר תפקוד מלא באמצעות מקלדת.
    * 2.2 יש לתת למשתמשים מספיק זמן לקרוא ולהשתמש בתכנים.
    * 2.3 אין לעצב תכנים באופן הידוע כגורם להתקפים.
    * 2.4 יש לספק דרכים כדי לעזור למשתמשים לנווט, לאתר תכנים, ולקבוע את מקום הימצאם.
-->

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---


# WCAG Understandable

## ניתן להבנה

- Make text readable and understandable.
- Make content appear and operate in predictable ways.
- Help users avoid and correct mistakes.
<!--    
* 3 ניתן להבנה
    * 3.1 יש ליצור תכני טקסט קריאים וניתנים להבנה.
    * 3.2 יש לגרום לדפי רשת להופיע ולתפקד באופן הניתן לניבוי.
    * 3.3 יש לסייע למשתמשים להימנע משגיאות ולתקנן.
-->

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# WCAG Robust

## יציב

- Maximize compatibility with current and future user tools.
<!--   
* 4 יציב
    * 4.1 יש לדאוג לתאימות מירבית עם סוכני משתמש קימים ועתידיים, כולל טכנולוגיות תומכות.
-->

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# WCAG in law

By Law: https://www.w3.org/WAI/policies/

The Israeli accessibility regulations were amended in 2017 to require web accessibility in all services provided over the internet. Both private and public entities providing services online are required to apply Internet Accessibility Standard (Israel Standard 5668), which has adopted WCAG 2.0. The regulations apply to both websites, at AA level, and to applications and to digital documents uploaded after Oct 2017. Personal information – such as bank client’s statements – is to be made accessibly by 2022. Accessible websites and apps are required to include an accessibility statement.
<br/><br/>
Captions are required for time-based media (Level A) uploaded after 2017. However, only public authorities and large-scale private businesses have to provide them. In addition, lectures, conferences and similar events presented online, may offer a text document as alternative to online accommodations. Services provided or promoted through social media are required to use the accessibility features offered by the platforms. Websites which host third-party content have to provide accessibility options, such as alt text descriptions for images.

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# How to use A11y software

Softwares:

- Jaws
- NVDA
- VoiceOver [keys](https://help.apple.com/voiceover/command-charts/)

https://www.tpgi.com/basic-screen-reader-commands-for-accessibility-testing/

Arrow keys - navigate
Tab key - jump to next focusable element (element should trigger smth, not just read)
https://www.magentaa11y.com/demos/basic-accessible-webpage/<br/>
https://www.magentaa11y.com/<br/>
https://play.tailwindcss.com/K02GpXc3ts<br/>

<!--   
Run voice over on demo website & leumi
Dom order focus
Tab key bad example - welcome text (accounts combo)
-->


---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# Semantic HTML5 and Aria
<div class="text-center">
  <img src="/imgs/semantic-twit.jpg" class="inline h-[280px]" />
  <img src="/imgs/non-semantic.png" class="inline h-[280px]" />
</div>

https://www.semrush.com/blog/semantic-html5-guide/

The difference between semantic and non-semantic tags may not seem important to sighted users, but it matters considerably to blind users for many reasons. In this example, the
tag informs the screen reader of a major set of navigation links. Semantic elements come with their own keyboard accessibility built-in, so no extra work is required on the user’s part.If you want to know which HTML element to use for each situation. [List of all elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

<!--
* seo benefits
* we will see later how ul, ol and other tags are helping us and we will prefer them most of the times
-->

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# Roles

ARIA roles provide semantic meaning to content.

https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles

Types:
- Document structure roles (toolbar, tooltip, none, cell, group, heading)
- Widgets (searchbox, slider, switch, menu, tabpanel, combobox)
- Landmark roles (banner, contentinfo, complementary, search)
- Live region (alert, log, status)
- Window (dialog, alertdialog)


---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# focus-visible

https://play.tailwindcss.com/5ZdPdCvzXi <br/>
https://tailwindcss.com/docs/hover-focus-and-other-states#hover-focus-and-active

```html
    <button type="button" class="
      ... 
      focus:outline-none 
      focus:ring-2 
      focus:ring-indigo-500 
      focus:ring-offset-2
    ">
      Focus button
    </button>

    <button type="button" class="
      ...
      focus:outline-none
      focus-visible:ring-2
      focus-visible:ring-indigo-500
      focus-visible:ring-offset-2
    ">
      Focus visible button
    </button>
```
<!--
* styling focus, outline - is important
* hover styles for focus but not always
* we are responsible to make sure focus is styled, designers miss it most of time
* focus-within
* devtools + states e.g active
-->

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# Focus trap
https://a11y-solutions.stevenwoodson.com/solutions/focus/modals/

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
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
<!--
* tabindex not removing element from sr, but only removes focusability
* eslint jsx-a11y plugin https://github.com/jsx-eslint/eslint-plugin-jsx-a11y
-->
---
class: "bg-[url(/imgs/bg.png)] bg-cover"
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
  aria-disabled="true"
  aria-pressed="false">
  Toggle
</div>
```
<!--
aria-disabled can be useful for styling, as works different from disabled
-->

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# Link anti-pattern

Anything that behaves like a link should use an `<a>` tag with an href, anything else should use a `<button>`

```jsx{1-6|7|10-14}
<button 
  type="button" 
  onClick={() => window.location.href="https://leumi.co.il"}>
  button
</button>

<a href="http://google.com">link</a>

<button 
  role="link" 
  type="button" 
  onClick={() => window.location.href="https://leumi.co.il"}>
  or at least use role="link" so SR will see it as a link
</button>
```
---
class: "bg-[url(/imgs/bg.png)] bg-cover"
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

https://www.aditus.io/patterns/multiple-navigation-landmarks/
```

or use aria:
```html
<div role="navigation" aria-label="Main">
  <!-- list of links to main website locations -->
</div>
```

## role=menu|menubar|menuitem are desktop menus
https://adrianroselli.com/2017/10/dont-use-aria-menu-roles-for-site-nav.html

<!--
* Without ul & li it wont be list
* Maybe open digital asakim old version 4 - show nav without ul
* Explain what is menubar
-->

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
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
class: "bg-[url(/imgs/bg.png)] bg-cover"
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

<!--
The role “none” was added to act as an alias for role=”presentation”, and both are the same and perform the same action. This was meant to provide clarity for those who were confused by the word “presentation.”
-->

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
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

https://tailwindcss.com/docs/screen-readers


---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# aria-label

#### The aria-label should be used to provide a text alternative to an element that has no visible text on the screen

```jsx{1|2|3-4|5-6|7-8}
<button>send</button> // accessible name: send
<button aria-label="send form">send</button> // accessible name: send form
<button aria-label="send button">...<button>// ⛔ BAD: "send button, button"
<button aria-label="send">...<button>// ✅ Good: "send, button"
<nav aria-label="primary">...</nav>
<nav aria-label="secondary">...</nav>
<button aria-label="Send">Send</button>// ⛔ BAD: over-using aria-label
<button>Send</button>// ✅ GOOD: use it only when needed it
```
<img src="/imgs/label-burger.png" class="h-[60px] my-3" /> 

<!--
If an element has both aria-labelledby and aria-label, the value of aria-labelledby will be used in the text alternative computation.
-->

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# aria-label vs. title


The title attribute shows as a tooltip when the mouse goes over the element. While it can be useful for people using the mouse, it will not be available to keyboard-only users. Note that while title attribute is listed in the text-alternative computation algorithm, it might not be supported in some combinations of screen-reader/browsers (at the time of writting, IE 11 and NVDA).

In short, If you find yourself using the title attribute to provide additional information, it's probably better to either use aria-label or think of an alternative (e.g.: disclosure additional information to users such as a tooltip).

```html
<a href=".." title="Washington stimulates economic growth">Read more</a>
<a href=".." title="Washington stimulates economic growth">
  <span class="sr-only">Washington stimulates economic growth </span>Read more
</a>
```

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# `<label>`

```html
<label for="firstname">First name:</label>
<input type="text" name="firstname" id="firstname">

<label>First name: <input type="text" name="firstname"></label>
```

### Get unique id in React

```jsx
import { useId } from 'react';

function Example(){
  const uniqueLabelId = useId();
  return (<>
    <label for={uniqueLabelId}>First name:</label>
    <input type="text" name="firstname" id={uniqueLabelId}>
  </>)
}
```

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# aria-labelledby
#### When label text is visible on screen, you should use aria-labelledby instead of aria-label.

```html{1-3|6-8|13,15-16,19-20}
// ⛔ BAD: using aria-label when text
<nav aria-label="Related Content">
  <h2>Related Content</h2>
  <ul>..</ul>
</nav>
// ✅ Good: using aria-labelledby when text
<nav aria-labelledby="nav-title">
  <h2 id='nav-title'>Related Content</h2>
  <ul>...</ul>
</nav>

<fieldset>
  <legend id="shipping-id">Billing</legend>
  <div>
    <div id="first-name">First Name</div>
    <input type="text" aria-labelledby="shipping-id first-name" />
  </div>
  <div>
    <div id="last-name">Address</div>
    <input type="text" aria-labelledby="shipping-id last-name" />
  </div>
</fieldset>
```

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# aria-labelledby & `<label>`

This is much like using a label element, with some key differences

- `aria-labelledby` may be used on any element, not just labelable elements
- While a `label` element refers to the thing it labels, the relationship is reversed in the case of `aria-labelledby` — the thing being labeled refers to the thing that labels it
- Only one label element may be associated with a labelable element, but `aria-labelledby` can take a list of IDREFs to compose a label from multiple elements. The label will be concatenated in the order that the IDREFs are given
- You can use `aria-labelledby` to refer to elements that are hidden and would otherwise not be in the accessibility tree. For example, you could add a hidden `span` next to an element you want to label, and refer to that with `aria-labelledby`
- However, since ARIA only affects the accessibility tree, `aria-labelledby` does not give you the familiar label-clicking behavior you get from using a `label` element  

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# Relationships


`aria-labelledby` is an example of a relationship attribute. A relationship attribute creates a semantic relationship between elements on the page regardless of their DOM relationship. In the case of `aria-labelledby`, that relationship is "this element is labelled by that element".

The ARIA specification lists eight relationship attributes. Six of these, `aria-activedescendant`, `aria-controls`, `aria-describedby`, `aria-labelledby`, and `aria-owns`, take a reference to one or more elements to create a new link between elements on the page. The difference in each case is what that link means and how it is presented to users.

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# aria-owns

When a parent/child relationship is evident on-screen, but it isn’t represented in the DOM, the aria-owns attribute can be used to establish that relationship in the accessibility layer


```html{1-9|5-9|2,6|11-21|13,17}
<ul>
  <li aria-owns="child">Fruit</li>
  <li>Vegetables</li>
</ul>

<ul id="child">
  <li>Apples</li>
  <li>Bananas</li>
</ul>

<input 
  aria-expanded="false" 
  aria-owns="autcomplete_list" 
  name="input-autocomplete" 
  type="text">
<ul 
  id="autcomplete_list" 
  role="listbox">
  <li aria-selected="false" role="option" aria-posinset="1" aria-setsize="7">Belarus</li>
  <li aria-selected="false" role="option" aria-posinset="2" aria-setsize="7">Belgium</li>
</ul>
```

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# aria-controls

The aria-controls attribute identifies the element (or elements) whose contents or presence are controlled by the element on which the attribute is set, regardless of what type of interaction initiates the impacted behavior

https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/tablist_role#keyboard_interactions

```html{all|2-15|16-17|5,16|11,17}
<div class="tab-interface">
  <div role="tablist" aria-label="Sample Tabs">
    <span role="tab" id="tab-1"
      aria-selected="true"
      aria-controls="panel-1"
      tabindex="0">
      First Tab
    </span>
    <span role="tab" id="tab-2"
      aria-selected="false"
      aria-controls="panel-2"
      tabindex="-1">
      Second Tab
    </span>
  </div>
  <div id="panel-1" role="tabpanel" tabindex="0" aria-labelledby="tab-1">...</div>
  <div id="panel-2" role="tabpanel" tabindex="0" aria-labelledby="tab-2" class="hidden">...</div>
</div>
```

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# aria-activedescendant

The aria-activedescendant attribute identifies the currently active element when focus is on a `composite` widget, `combobox`, `textbox`, `group`, or `application`.


```html{all|5,11}
<input 
  aria-expanded="false" 
  aria-owns="autcomplete_list" 
  name="input-autocomplete" 
  aria-activedescendant="belgium"
  type="text">
<ul 
  id="autcomplete_list" 
  role="listbox">
  <li id="belarus" aria-selected="false" role="option" aria-posinset="1" aria-setsize="7">Belarus</li>
  <li id="belgium" aria-selected="false" role="option" aria-posinset="2" aria-setsize="7">Belgium</li>
</ul>
```
---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# aria-describedby

```html{1-4|1-2|5-8|7,8|9-17|13,16}
<button aria-describedby="trash-desc">Move to trash</button>
<p id="trash-desc">
  Items in the trash will be permanently removed after 30 days.
</p>

<label for="fname">First name</label>
<input name="fname" type="text" id="fname" aria-describedby="hint">
<p id="hint">A bit of instructions for this field linked with aria-describedby. </p>

<input type="text" id="first" name="first"
      onmouseover="tooltipShow()"
      onfocus="tooltipShow()"
      aria-describedby="hint-tooltip"
      aria-required="false"/>

<div id="hint-tooltip" role="tooltip" aria-hidden="true">Your first name is optional. </div>
```
---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# form validation


```html
<label for="email">Your email</label>
<input type="text" id="email" aria-invalid="true" aria-describedby="emailHint emailError">
<p id="emailHint">gmail is forbidden</p>
<p id="emailError" role="alert">Invalid email address.</p>
```
https://www.w3.org/WAI/tutorials/forms/

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# aria-current
The aria-current attribute should be used to identify the current item in a set of items. Below we show some applications of this attribute to make websites more accessible to all users

values: page, step, location, date, time, false, true
<div class="text-center">
  <img src="/imgs/aria-current-page-vo.png" class="h-[160px] inline" />
  <img src="/imgs/aria-current-location-vo.png"  class="h-[160px] inline" />
  <img src="/imgs/aria-current-date.png"  class="h-[160px] inline" />
  <img src="/imgs/aria-current-step.png"  class="h-[160px] inline" />
</div>
---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# aria-current code examples

```html{all|16}
<nav aria-label="breadcrumbs">
  <ol>
    <li>
      <a href="/">
        Home
      </a>
    </li>
    <li>
      <a href="/parent">
        Parent
      </a>
    </li>
    <li>
      <a
        href="/parent/current"
        aria-current="location"
      >
        Current
      </a>
    </li>
  </ol>
</nav>
```
---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# aria-current vs. aria-selected

In widgets where aria-selected has the same meaning as aria-current, we should use aria-selected instead.

For example, when using Tabs, we should mark the currently selected tab with aria-selected="true. This has the same meaning as aria-current="page", but aria-selected="true" is preferred.

```html{all|2}
 <div role="tablist" aria-label="Entertainment">
  <button id="tab-1-button" role="tab" aria-controls="tab-1" aria-selected="true">
    Tab 1
  </button>
  <button id="tab-2-button" role="tab" aria-controls="tab-2">
    Tab 2
  </button>
</div>

<div id="tab-1" 
    role="tabpanel"
    tabindex="0" 
    aria-labelledby="tab-1-button"
>...</div>
<div id="tab-2" role="tabpanel"
    tabindex="0" 
    aria-labelledby="tab-2-button"
    hidden>...</div>
```

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---
# aria-expanded

The aria-expanded attribute is set on an element to indicate if a control is expanded or collapsed, and whether or not its child elements are displayed or hidden

```jsx
<button
  aria-expanded="false"
  aria-controls="username-desc"
  aria-label="Help about username"
  onClick={()=>setOpen(val=>!val)}
  type="button">
  <span aria-hidden="true">?</span>
</button>

<p id="username-desc" hidden={open}>
  Your username is the name that you use to log in to this service.
</p>
```

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---
# aria-haspopup
The aria-haspopup attribute indicates the availability and type of interactive popup element that can be triggered by the element on which the attribute is set

- true == menu
- menu
- listbox
- tree
- grid
- dialog

```html
<button aria-expanded="false" aria-haspopup="true" aria-controls="menu-id">Toggle Menu</button>     
<ul id="menu-id" role="menu" aria-hidden="true">...</ul>
```

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# aria-live
Dynamic content which updates without a page reload is generally either a region or a widget. Simple content changes which are not interactive should be marked as live regions. A live region is explicitly denoted using the aria-live attribute.


aria-live="assertive" == role="alert"
most of the time we will use aria-live="polite". The screen reader will speak changes whenever the user is idle

https://bitsofco.de/using-aria-live/
https://codepen.io/joe-watkins/pen/NWOxov


---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# aria-atomic

As an illustration of aria-atomic, consider a site with a simple clock, showing hours and minutes. The clock is updated each minute, with the new remaining time overwriting the current content
```html
<div id="clock" role="timer" aria-live="polite" aria-atomic="true">…</div>
```
aria-atomic="true" ensures that each time the live region is updated, the entirety of the content is announced in full (e.g. "17:34").

Another example of aria-atomic - an update/notification made as a result of a user action

```jsx
<div id="date-input">
  <label for="year">Year:</label>
  <input type="text" id="year" value="1990" onBlur={(e)=>setYear(event.target.value)} />
</div>

<div id="date-output" aria-atomic="true" aria-live="polite">
  The set year is:
  <span id="year-output">{year}</span>
</div>
```

https://codepen.io/fstorr/full/rxbZyG
---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# aria-busy

indicates an element is being modified and that assistive technologies may want to wait until the changes are complete before informing the user about the update.

Temporarily stop updates being announced while busy:
```html
<ol aria-live="polite" aria-busy="true">⋯</ol>
```

Loaders:

```jsx
<div id="loader">
  <SomeCoolLoader aria-hidden="true" />
  <p class="sr-only">Please wait while the content is loading...</p>
</div>

<div aria-busy="true">
  <!-- Loading content goes here -->
</div>
```

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---
# Checkbox

```jsx
<label>
  <input type="checkbox" class="sr-only" />
  <div class="checkbox_visual" />
  <span>Basic checkbox</span>
</label>
```

https://play.tailwindcss.com/WNbicnwwhK
---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---
# Radio 

```jsx
<label>
  <input type="radio" class="sr-only" />
  <div class="radio_visual" />
  <span>Basic checkbox</span>
</label>
```
https://play.tailwindcss.com/fSOVuJh2E8
---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---
# Accordion

```jsx
function AccordionItem({ id, title, children }) {
  const [isExpanded, setIsExpanded] = useState(false);
  return (
    <>
      <h3>
        <button
          id={`${id}-header`}
          aria-controls={`${id}-panel`}
          aria-expanded={isExpanded}
        >{title}</button>
      </h3>
      <section
        id={`${id}-panel`}
        aria-labelledby={`${id}-header`}
        hidden={!isExpanded}
      >{children}</section>
    </>
  )
}
// usage
<AccordionItem id='item-1' title='Section title'><-- content goes here --></AccordionItem>
```

https://www.aditus.io/patterns/accordion/

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---
# Whisper

```jsx{all|3|4|4,6,2}
<Whisper 
  speaker={<Popover>Export data</Popover>} 
  trigger={["hover", "focus"]} // set by default
  controlId="export-example" // if not provided will be generated
  >
  <IconButton // has to be "focusable" element
    circle
    icon={<DownloadIcon />}
  />
</Whisper>
```

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---
# Dropdowns

```html
<div class="a11y-container">
  <p id="a11y-usage-select-element-js" class="sr-only">Utilisez la tabulation (ou les touches flèches) pour naviguer dans la liste des suggestions</p>
  <label for="a11y-select-element-js" class="sr-only">Rechercher dans la liste</label>
  <input type="text" id="a11y-select-element-js" aria-describedby="a11y-usage-select-element-js">
  <div id="a11y-select-element-suggestions" role="listbox" aria-multiselectable="true">
    <div role="option" tabindex="0" data-index="0" class="a11y-suggestion">Sleeping</div>
    <div role="option" tabindex="0" data-index="1" class="a11y-suggestion" aria-selected="true">Climbing trees</div>
    <div role="option" tabindex="0" data-index="2" class="a11y-suggestion">Knitting socks</div>
    <div role="option" tabindex="0" data-index="3" class="a11y-suggestion" aria-selected="true">Riding bikes</div>
    <div role="option" tabindex="0" data-index="4" class="a11y-suggestion">Eating cupcakes</div>
</div>
</div>
```
https://www.magentaa11y.com/checklist-web/select/
https://github.com/alphagov/accessible-autocomplete


---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# Basic table


<table>
<caption>Monthly Budget</caption>
  <thead>
    <tr>
      <th scope="col">Month</th>
      <th scope="col">Amount Earned</th>
      <th scope="col">Amount Spent</th>
			<th scope="col">Amount Saved</th>
    </tr>
  </thead>
  <tbody>
    <tr>
			<th scope="row">January</th>
			<td>$2500</td>
			<td>$1500</td>
			<td>$500</td>
    </tr>
		<tr>
			<th scope="row">February</th>
			<td>$2700</td>
			<td>$1500</td>
			<td>$700</td>
		</tr>
  </tbody>
</table>

https://www.w3.org/WAI/tutorials/tables/


---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---
# Basic table

```html
<table>
<caption>Monthly Budget</caption>
  <thead>
    <tr>
      <th scope="col">Month</th>
      <th scope="col">Amount Earned</th>
      <th scope="col">Amount Spent</th>
      <th scope="col">Amount Saved</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">January</th>
      <td>$2500</td>
      <td>$1500</td>
      <td>$500</td>
    </tr>
    <tr>
      <th scope="row">February</th>
      <td>$2700</td>
      <td>$1500</td>
      <td>$700</td>
    </tr>
  </tbody>
</table>
```

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---
# Basic table

```html
<div role="table" aria-label="Monthly Budget"> <!-- <table> -->
  <div role="rowgroup">
    <div role="row">
      <div role="columnheader">Month</div>
      <div role="columnheader">Amount Earned</div>
      <div role="columnheader">Amount Spent</div>
      <div role="columnheader">Amount Saved</div>
    </div>
    <div role="row">
      <div role="rowheader">January</div>
      <div role="cell">$2500</div>
      <div role="cell">$1500</div>
      <div role="cell">$500</div>
    </div>
    <div role="row">
      <div role="rowheader">February</div>
      <div role="cell">$2700</div>
      <div role="cell">$1500</div>
      <div role="cell">$700</div>
    </div>
  </div>
</div>
```
---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# Reduced motion
<div class="text-center">
  <img src="/imgs/reduced-motion.png" class="inline mb-2 h-[200px]" />
</div>

```css
@media screen and (prefers-reduced-motion: reduce) {
   .theheart, .firststrokes {
       animation: none;
   }
   .secondstrokes, .explode, .explode2 {
       display: none;
   }
}
```

https://youtu.be/-7ENwVFOh_I

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# Devtools 

- [Lighthouse](https://developer.chrome.com/docs/devtools/accessibility/reference/)
- [aXe extension](https://chrome.google.com/webstore/detail/axe-devtools-web-accessib/lhdoppojpmngadmnindnejefpokejbdd) 
- Accessibility panel in chrome devtools (+ experimental full-page accessibility tree)
- [Contrast check](https://developer.chrome.com/docs/devtools/accessibility/contrast/)
- Rendering: emulate vision deficiencies, reduced motion, prefer contrast, dark mode and etc.

---
class: "bg-[url(/imgs/bg.png)] bg-cover"
---

# Useful links

https://www.smashingmagazine.com/2021/03/complete-guide-accessible-front-end-components/
