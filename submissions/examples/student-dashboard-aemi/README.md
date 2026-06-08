# ease-student-dashboard-aemi

> An interactive, animated Student Academic & Portfolio Dashboard component built entirely with EaseMotion CSS utilities and custom CSS — zero JavaScript.

---

## Preview

A dark-themed, responsive dashboard containing:

| Section | Description |
|---------|-------------|
| **Header** | Gradient title with animated avatar using `ease-hover-grow` |
| **Skill Marquee** | Infinite scrolling tech-stack badges using `ease-marquee` + pause-on-hover |
| **Project Cards** | Multi-column animated project cards with `ease-hover-lift` + `ease-slide-up` |
| **Schedule Card** | Today's class timeline with styled time badges |
| **Stats Card** | Key academic metrics with animated gradient numbers using `ease-pulse` |

---

## EaseMotion Classes Used

| Class | Effect |
|-------|--------|
| `ease-fade-in` | Page entrance fade for the dashboard wrapper |
| `ease-slide-up` | Cards animate upward on load |
| `ease-delay-100/200/300` | Staggered entrance for each card |
| `ease-hover-lift` | Cards lift with a glow shadow on hover |
| `ease-hover-grow` | Avatar scales up on hover |
| `ease-pulse` | CGPA stat pulses subtly to draw attention |

---

## Usage

```html
<!-- Link EaseMotion CSS -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/easemotion-css/easemotion.min.css" />

<!-- Link component styles -->
<link rel="stylesheet" href="style.css" />

<!-- Drop in the component -->
<div class="student-dashboard ease-fade-in">
  ...
</div>
```

---

## Customization

Override any CSS variable to retheme the dashboard instantly:

```css
:root {
  --dash-bg:      #0a0a0a;    /* Background */
  --dash-accent:  #f97316;    /* Orange accent */
  --dash-accent2: #ec4899;    /* Pink gradient */
}
```

---

## Submission Details

- **Author:** 24CS059Aemi
- **GSSoC '26** Contributor
- **Related Issue:** [#2738](https://github.com/SAPTARSHI-coder/EaseMotion-css/issues/2738)
- **Files:** `demo.html` · `style.css` · `README.md`
- **Naming:** Uses unique suffix `-aemi` per contribution policy
