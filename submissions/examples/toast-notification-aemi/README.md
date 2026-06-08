# ease-toast-notification-aemi

> Glassmorphism animated toast notification component — 4 variants, CSS-only toggle, progress bar, and accessibility support. Zero JavaScript required.

---

## Preview

| Variant | Trigger | Color |
|---------|---------|-------|
| ✅ **Success** | Click button | Green glow |
| ⚠️ **Warning** | Click button | Amber glow |
| ❌ **Error** | Click button | Red glow |
| ℹ️ **Info** | Click button | Blue glow |
| ⬆️ **Progress** | Always visible | Purple animated bar |

Toasts **slide in** from the right with a spring bounce effect and **slide out** on close. The progress bar animates in a loop.

---

## EaseMotion Classes Used

| Class | Effect |
|-------|--------|
| `ease-fade-in` | Page entrance animation |
| `ease-slide-up` | Demo title & subtitle entrance |
| `ease-delay-100/200/300` | Staggered entrance timing |

---

## Usage

```html
<!-- 1. Link EaseMotion CSS -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/easemotion-css/easemotion.min.css" />

<!-- 2. Link component styles -->
<link rel="stylesheet" href="style.css" />

<!-- 3. Add a hidden checkbox (CSS-only toggle) -->
<input type="checkbox" id="my-toast-toggle" class="toast-trigger" />

<!-- 4. Add trigger button -->
<label for="my-toast-toggle">Show Toast</label>

<!-- 5. Add toast container + toast -->
<div class="ease-toast-container">
  <div class="ease-toast ease-toast-success" id="my-toast">
    <div class="toast-icon">✅</div>
    <div class="toast-content">
      <strong>Success!</strong>
      <span>Your action was completed.</span>
    </div>
    <label class="toast-close" for="my-toast-toggle">✕</label>
  </div>
</div>
```

---

## Variants

```html
<!-- Success -->
<div class="ease-toast ease-toast-success"> ... </div>

<!-- Warning -->
<div class="ease-toast ease-toast-warning"> ... </div>

<!-- Error -->
<div class="ease-toast ease-toast-error"> ... </div>

<!-- Info -->
<div class="ease-toast ease-toast-info"> ... </div>

<!-- With progress bar -->
<div class="ease-toast ease-toast-progress">
  <div class="toast-content">
    <strong>Uploading...</strong>
    <div class="ease-progress-bar">
      <div class="ease-progress-fill"></div>
    </div>
  </div>
</div>
```

---

## Customization

Override CSS variables to retheme instantly:

```css
:root {
  --toast-radius:   10px;          /* Corner rounding */
  --toast-blur:     24px;          /* Glassmorphism blur amount */
  --toast-duration: 0.5s;          /* Slide-in/out speed */
}
```

---

## Accessibility

Respects `prefers-reduced-motion` — all transitions and animations are disabled automatically for users who prefer reduced motion:

```css
@media (prefers-reduced-motion: reduce) {
  .ease-toast { transition: none; }
}
```

---

## Submission Details

- **Author:** 24CS059Aemi
- **GSSoC '26** Contributor
- **Naming:** Unique suffix `-aemi` per contribution policy
- **Files:** `demo.html` · `style.css` · `README.md`
- **No edits** to `core/` or `components/`
