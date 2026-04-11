# Fedora – Come mettere online il sito

## 1. Crea il repository e carica i file
1. Su GitHub crea un nuovo repository pubblico
2. Carica dentro: `index.html`, `trasparenza.html`, `logo.png` (se vuoi)
3. Clicca **Commit changes**

---

## 2. Attiva GitHub Pages
1. Vai su **Settings** del repository
2. Menu a sinistra → **Pages**
3. Branch: **main** → cartella **/ (root)** → **Save**

Il sito è già online su `https://tuonome.github.io/nome-repository/`

---

## 3. Collega il dominio
1. Sempre in **Settings → Pages**, campo **Custom domain** → scrivi `www.tuodominio.qualocsa` → **Save**
2. Vai nel pannello DNS del tuo registrar (Aruba, Register, GoDaddy…)
3. Aggiungi questi record:

| Tipo  | Nome | Valore            |
|-------|------|-------------------|
| A     | @    | 185.199.108.153   |
| A     | @    | 185.199.109.153   |
| A     | @    | 185.199.110.153   |
| A     | @    | 185.199.111.153   |
| CNAME | www  | tuonome.github.io |

4. Aspetta 10–30 minuti
5. Torna su GitHub Pages e spunta **Enforce HTTPS**
