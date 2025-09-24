# 🎨 Mini Style Guide – Portfolio Page

## 1. Typography

- **Fonts**
  - Heading: `Poppins`, sans-serif
  - Body: `Roboto`, sans-serif
- **Scale (rem-based, via CSS variables)**

```css
:root {
  /* Font Sizes */
  --size-xxs: 0.5rem;
  --size-xs: 0.75rem;
  --size-sm: 0.875rem;
  --size-base: 1rem;
  --size-lg: 1.125rem;
  --size-xl: 1.25rem;
  --size-2xl: 1.5rem;
  --size-3xl: 1.875rem;
  --size-4xl: 2.25rem;
  --size-5xl: 3rem;
  --size-6xl: 3.75rem;
  --size-7xl: 4.5rem;
  --size-8xl: 6rem;
  --size-9xl: 8rem;
  --size-10xl: 10rem;
}
```

- **Hierarchy Example**
  - Hero title: `--size-4xl` – `--size-5xl`
  - Section title / Subtitle: `--size-2xl` – `--size-3xl`
  - Sub sub-title: `--size-lg` – `--size-xl`
  - Body: `--size-base`

---

## 2. Color Palette

### Light Theme

```css
:root {
  --color-bg: #f9fafb;
  --color-surface: #ffffff;
  --color-text: #111827;
  --color-text-secondary: #4b5563;
  --color-accent: #2563eb;
  --color-accent-alt: #38bdf8;
}
```

### Dark Theme

```css
[data-theme='dark'] {
  --color-bg: #111827;
  --color-surface: #1f2937;
  --color-text: #f9fafb;
  --color-text-secondary: #d1d5db;
  --color-accent: #60a5fa;
  --color-accent-alt: #38bdf8;
}
```

### Status Labels

```css
:root {
  --color-success: #22c55e;
  --color-warning: #f59e0b;
  --color-future: #6b7280;
}
```

---

## 3. Spacing System

- **Base unit:** 4px (~0.25rem)
- **Semantic aliases (map to scale):**

```css
:root {
  --space-sm: 0.1rem;
  --space-md: 0.2rem;
  --space-lg: 0.3rem;
  --space-xl: 0.4rem;
}
```

- **Border radius:** 8px default, 9999px pill
- **Shadow:**

```css
--shadow-sm: 0 1px 2px rgba(0, 0, 0, 0.05);
--shadow-md: 0 4px 6px rgba(0, 0, 0, 0.1);
--shadow-lg: 0 10px 15px rgba(0, 0, 0, 0.15);
```

---

## 4. Naming Convention (Hybrid)

- **BEM** → untuk section/component khusus
  - `.hero__title`, `.skills__card--current`
- **Generic** → untuk reusable pattern
  - `.btn`, `.title`, `.sub-title`, `.container`
- **Utilities** → untuk helper cepat
  - `.text-center`, `.mt-lg`, `.hidden`

### Rule of Thumb

- Section-specific? → **BEM**
- Dipakai di banyak tempat? → **Generic**
- Hanya 1 properti inline kecil? → **Utility**

---

## 5. Checklist Usage

✅ Typography pakai `Poppins + Roboto` + rem scale  
✅ Gunakan **dark mode palette default** (light ready untuk future)  
✅ Spacing konsisten pakai semantic alias  
✅ Card & button → radius 8px, shadow minimal  
✅ Class naming → patuhi hybrid convention  
✅ CTA button & section headings konsisten

---

⚙️ **Rule**:  
Sebelum mulai styling, cek semua checklist ini → jangan skip, biar hasil clean & industry-ready.
