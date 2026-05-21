# Try Before Pay — Demo Website

Statikus, többoldalas demó a féléves projektzáró dokumentációhoz.
**Csapat:** Kovalik B., Török D., Balla A., Gimes Sz.

## Tartalom (oldalak)
1. **index.html** — One-pager + élő checkout demó
2. **problem.html** — Probléma leírása
3. **segment.html** — Ügyfélszegmens
4. **vision.html** — Vízió, misszió, értékek
5. **bmc.html** — Business Model Canvas
6. **pricing.html** — Árazás &amp; bevételi modell
7. **feasibility.html** — Megvalósíthatóság &amp; interaktív break-even kalkulátor

Nincs build lépés, nincs függőség. Tisztán HTML + CSS + JS.

---

## Lokálisan megnyitni
Csak nyisd meg az `index.html`-t a böngészőben (dupla kattintás).
Vagy futtass egy mini szervert (PowerShell):

```powershell
cd h:\TryBeforePay-Demo
python -m http.server 8080
# majd: http://localhost:8080
```

---

## Publikálás — 3 egyszerű lehetőség

### 1) Netlify Drop (legegyszerűbb, kb. 30 mp)
1. Menj a https://app.netlify.com/drop oldalra
2. Húzd be a teljes `TryBeforePay-Demo` mappát az ablakba
3. Kapsz egy nyilvános linket (pl. `https://random-name.netlify.app`)
4. (Opcionális) "Site settings → Change site name" → személyre szabhatod, pl. `try-before-pay.netlify.app`

**Nem kell regisztráció sem** az ideiglenes linkhez, de ha megtartanád, jelentkezz be GitHub vagy email accountal.

### 2) Vercel (szintén drag & drop)
1. https://vercel.com → Sign up GitHubbal
2. "Add New → Project → Import" vagy húzd be a mappát a CLI-vel: `npx vercel`
3. Kapsz egy `*.vercel.app` linket

### 3) GitHub Pages (ha GitHubot használtok)
```powershell
cd h:\TryBeforePay-Demo
git init
git add .
git commit -m "Try Before Pay demo site"
git branch -M main
git remote add origin https://github.com/<felhasznalonev>/try-before-pay.git
git push -u origin main
```
Majd a repo `Settings → Pages → Source: main / root` → kapsz egy `https://<felhasznalonev>.github.io/try-before-pay/` linket.

---

## Mit küldj be a Moodle-ra?
- Töltsd fel a publikus linket szövegként a beadásba **VAGY**
- Csomagold ZIP-be a `TryBeforePay-Demo` mappát és add be mellékletként
- A meglévő PDF / PPTX / XLSX dokumentumokat változatlanul mellékelheted

A weboldalon **a csapattagok neve minden oldal alján** szerepel.
