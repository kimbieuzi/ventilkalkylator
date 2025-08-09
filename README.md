# SAMSON Ventilkalkylator – GitHub Pages

Det här paketet är klart att publicera som **GitHub Pages** (live-länk).

## Innehåll
- `index.html` – kalkylatorn (v4.1, failsafe)
- `samson_product_library_exact.csv` – exempel på produktbibliotek
- `assets/samson_logo.jpeg` – logga som kan användas i UI:t
- `.nojekyll` – gör att GitHub inte kör Jekyll-processning
- `404.html` – enkel redirect tillbaka till startsidan

---

## Publicera (3 minuter)
1. Skapa ett nytt repo på GitHub, t.ex. **ventilkalkylator**.
2. Ladda upp **alla filer** i den här mappen (eller ladda upp ZIP:en och extrahera den i repos root).
3. Gå till **Settings → Pages**:
   - **Source:** *Deploy from a branch*
   - **Branch:** `main` (root)
4. Vänta 10–60 sekunder → din sida blir live på:
   `https://USERNAME.github.io/ventilkalkylator/`

> **Tips:** Om du redan har ett org/domän, lägg en `CNAME`-fil med din domän (valfritt).

---

## Så använder du kalkylatorn
- Öppna sidan → fliken **Vätska** (eller **Gas/Ånga (BETA)**).
- Mata in **Q, ΔP, SG** (+ öppningsgrad/karakteristik) → du får **Kv, Kvs**, och **≈DN**.
- Fliken **Produktförslag**: klicka *Produktbibliotek (CSV)* och ladda `samson_product_library_exact.csv`
  (eller er egen fil) för **exakta** modeller/trim och **databladslänkar**.
- **Skicka RFQ** via e-post eller använd **Skicka till CRM** (Inställningar → ange din webhook-URL).

### Branding
- I **Inställningar** kan du ange *Accentfärg* och *Logotyp URL*. För att använda medföljande logga:
  skriv in `/assets/samson_logo.jpeg` i fältet *Logotyp URL*.

### Vanliga frågor
- **Inget händer när jag öppnar sidan?** Du måste öppna den via den hostade länken.
  (Om du öppnar som fil i en förhandsvisare kan JavaScript blockeras.)
- **Safari/iOS privatsurfning?** v4.1 är fail-safe och fungerar även utan `localStorage`.
- **Gas/Ånga (BETA)?** Förenklad metod (icke-strypt). Bekräfta alltid mot IEC 60534-2-1 och datablad.
