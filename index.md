<!-- .slide: data-background="/images/background/00.svg" -->

# Accessible Web Mapping Apps

<p class="author">
    Kelly Hutchins<br>
    Tao Zhang
</p>

<p id="keyboardGuide">Press Space key for next slide</p>

---
<!-- .slide: data-background="/images/background/01.svg" -->

## What we will cover today

- Semantics
- Focus
- Keyboard
- Testing



---
<!-- .slide: data-background="/images/background/01.svg" -->

## Semantics

<p class="left-align">Choose the right HTML elements to reflect content *structure* and *meaning*.</p>



---
<!-- .slide: data-background="/images/background/01.svg" -->

### Structure

[MDN: HTML elements reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)



---
<!-- .slide: data-background="/images/background/01.svg" -->

## Focus

When part or all of the DOM gets updated by JavaScript, keyboard focus could be easily lost.

General approach:

1. Store a reference to currently focused element.
2. After rendering of new DOM, send focus back to previous element.
3. If 2 is not possible, send focus to the most meaningful element in the context.



---
<!-- .slide: data-background="/images/background/01.svg" -->

### JS API





---
<!-- .slide: data-background="/images/background/01.svg" -->

## Feedback 

- Internal stakeholders (SMEs, Dev, PE, etc.)
- Usability studies



---
<!-- .slide: data-background="/images/background/01.svg" -->

## Next steps

- Project milestones with due dates
- Team members required to move forward (UX, UI, PE, Dev, Project Manager, etc.)



---
<!-- .slide: data-background="/images/background/02.svg" -->

## Resources

- Link to Devtopia/GitHub issue (meeting notes, action items, design decisions, etc.)
- Project wiki
- InVision board for comparative research
- ...