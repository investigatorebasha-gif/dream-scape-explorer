## Modifica griglia campioni responsive

File: `public/museo/index.html` (CSS inline)

1. **Tablet (≤768px)** — riga 1801-1804: cambiare `.gallery-grid` da `repeat(2, …)` a `repeat(3, minmax(0, 1fr))`, ridurre `gap` a `16px`.

2. **Mobile (≤640px)** — riga 1920-1925: cambiare `.gallery-grid` da `1fr` a `repeat(4, minmax(0, 1fr))`, ridurre `gap` a `8px`, padding laterale `0 12px`.

3. **Card su mobile** — ridurre dimensioni testo/padding interni delle card per renderle leggibili a 4 per riga (font del titolo ~0.7rem, padding compatto, badge più piccoli). Modifiche scoped dentro il media query `(max-width: 640px)`.

4. **Desktop**: nessuna modifica (resta `repeat(4, …)`).

Nessuna modifica alla logica JS o alla struttura HTML.