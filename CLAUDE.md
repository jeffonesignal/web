# Claude Instructions

## Project: index.html Translation

### HTML Translation Structure
The `index.html` file contains 7 sequential `<p>` tags in the `<body>`. Their position determines their language — there are no `lang` or `data-lang` attributes:

```
<p>1. English (en) — source of truth</p>
<p>2. Simplified Chinese (cn)</p>
<p>3. Korean (ko)</p>
<p>4. Japanese (ja)</p>
<p>5. Portuguese (pt)</p>
<p>6. French (fr)</p>
<p>7. Turkish (tr)</p>
```

Example of current content:
```html
<p>Whether you're migrating from another platform...</p>   <!-- en -->
<p>无论你是从其他平台迁移过来...</p>                          <!-- cn -->
<p>다른 플랫폼에서 이전하는 경우든...</p>                      <!-- ko -->
<p>他のプラットフォームから移行する場合でも...</p>               <!-- ja -->
<p>Se você estiver migrando de outra plataforma...</p>     <!-- pt -->
<p>Que vous migriez depuis une autre plateforme...</p>     <!-- fr -->
<p>...</p>                                                 <!-- tr -->
```

### Translation Rules
- English (`en`) is always the source of truth
- Never alter HTML structure, only text content inside `<p>` tags
- Maintain formal/professional tone consistent with existing translations
- Languages to translate: en, cn, ko, ja, pt, tr, fr

### Commit Convention
- Translation commits: `chore: auto-translate p tags to cn, ko, ja, pt, tr, fr`