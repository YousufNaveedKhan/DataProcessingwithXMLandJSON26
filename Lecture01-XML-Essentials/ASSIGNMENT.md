# Assignment 1 — XML Essentials

**Topic:** jo Lecture 1 mein parha: XML basics, well-formed rules, entities/CDATA, attributes, default namespace, `sitemap.xml`.
**Tools:** VS Code + Chrome (ya Edge). Sab files **UTF-8** mein, extension **`.xml`** (Windows mein "File name extensions" ON rakho, warna `file.xml.txt` ban jati hai).

---

## Part A — Chhote sawal (apne alfaaz mein, 1-3 lines)

1. HTML aur XML mein **3 farq** likho.
2. XML ko "extensible" kyun kehte hain? Ek misaal do.
3. **Well-formed** aur **valid** XML mein kya farq hai?
4. XML document ki lifecycle ke 5 steps likho.
5. Namespace ki zaroorat kyun parti hai? Aur `xmlns="http://..."` wala URI kya browser/parser internet se download karta hai?

## Part B — Galtiyan dhoondo

Ye XML copy karke `broken.xml` mein save karo aur Chrome mein kholo:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<Shop>
  <product id=1>
    <name>Tea & Biscuits</name>
    <price>250</Price>
    <stock>Available<stock>
  </product>
  <3rd-party>no</3rd-party>
</Shop>
<owner>Ali</owner>
```

1. Browser ke error (line aur column) ko parh kar **ek ek galti** fix karo.
2. Theek ki hui file `fixed.xml` mein save karo.
3. `answers.txt` mein har galti ke liye likho: **kaun si line, kya galti thi, kya fix kiya, aur kaun sa rule toota.**

## Part C — `my-class.xml`

Apni class ka XML likho:

- Pehli line XML declaration (UTF-8)
- Root element `<class>` jis par `name` attribute ho (jaise `name="Semester 2 - Batch A"`)
- Kam az kam **4** `<student>` elements. Har ek par `id` attribute, aur andar `<name>`, `<city>`, `<marks>`
- Kam az kam **1 comment**
- Kisi ek value mein **`&`** ho (entity ke saath, jaise `Tom &amp; Jerry`)
- Aakhir mein ek `<note>` element jis ke andar **CDATA** block ho (jaise `<![CDATA[ marks < 40 matlab fail ]]>`)
- Chrome mein kholo, tree ka **screenshot** lo

> Ye file **sambhal kar rakho**, agle lecture mein isay JSON mein badlenge.

## Part D — `sitemap.xml`

Kisi website ke (apni, ya farzi) **4 pages** ka sitemap likho:

- Root `<urlset>` aur **default namespace** `http://www.sitemaps.org/schemas/sitemap/0.9`
- Har `<url>` mein `<loc>` (poora URL `https://...`) aur `<lastmod>` (format `YYYY-MM-DD`)
- Kam az kam ek URL aisa ho jis mein query ho aur uska `&` sahi tareeqe se likha ho (`?a=1&amp;b=2`)
- Chrome mein kholo, tree ka **screenshot** lo

## Part E — Bonus (zaroori nahi)

Koi chhoti `.docx` file copy karo, extension `.zip` karke extract karo, `word/document.xml` ko VS Code mein kholo. 2-3 lines likho ke aap ne kya dekha, aur screenshot lagao.

---

## Submit kya karna hai

Ek folder `AapkaNaam_XML_Assignment1` banao jis mein ye files hon:

| File | Part |
|---|---|
| `answers.txt` | Part A ke jawab + Part B ki galtiyon ki list |
| `broken.xml` aur `fixed.xml` | Part B |
| `my-class.xml` + screenshot | Part C |
| `sitemap.xml` + screenshot | Part D |
| bonus ka note + screenshot | Part E (agar kiya) |

Submit karwane ka tareeqa aur last date group mein bataya jayega.

## Submit karne se pehle check karo

- [ ] Har `.xml` file Chrome mein khulti hai aur tree dikhata hai (error nahi)
- [ ] Har file ki pehli line `<?xml version="1.0" encoding="UTF-8"?>` hai aur us se pehle koi space nahi
- [ ] Ek file mein sirf **ek root** element hai
- [ ] `&` aur `<` text mein entities ke saath likhe hain
- [ ] Naam sahi hain, extension `.xml` hai (`.xml.txt` nahi)
- [ ] Apna kaam khud kiya hai (copy-paste ki wajah se ek jaisi files pakri jati hain)
