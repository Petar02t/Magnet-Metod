# Magnet Metod — sajt za GitHub Pages

Ovaj folder je spreman da se direktno postavi na GitHub i objavi kao sajt (besplatno, preko GitHub Pages).

## Šta se nalazi u folderu

- `index.html` — glavna stranica sajta (svi CSS i JS su već unutra)
- `assets/` — sve slike i video snimci koje stranica koristi (23 fajla, ~18 MB ukupno)

Za razliku od fajla koji si ranije dobijao (jedan HTML od ~24 MB sa svime "ubačenim" unutra), ovde su slike i videi izdvojeni u posebne fajlove. To znači da će se sajt mnogo brže učitavati kad ode "u živo" (browser učitava resurse paralelno i kešira ih), što je bitno i za brzinu i za Google.

## Kako da objaviš sajt na GitHub Pages (korak po korak)

1. **Napravi novi repozitorijum na GitHub-u**
   Idi na github.com → **New repository** → daj mu ime (npr. `magnet-metod`) → **Create repository**.

2. **Otpakuj ovaj zip fajl** na svom računaru.

3. **Ubaci fajlove u repozitorijum**
   Najlakše je preko browsera: otvori svoj novi repozitorijum na GitHub-u → klikni **Add file → Upload files** → prevuci `index.html` i ceo `assets` folder unutra → **Commit changes**.

   (Ako koristiš git preko komandne linije, to je standardno: `git add .`, `git commit -m "Prvi sajt"`, `git push`.)

4. **Uključi GitHub Pages**
   U repozitorijumu idi na **Settings → Pages** (u levom meniju).
   Pod "Build and deployment" → **Source** izaberi **Deploy from a branch**.
   Pod "Branch" izaberi `main` i folder `/ (root)` → **Save**.

5. **Sačekaj 1-2 minuta**
   GitHub će ti dati link tipa:
   `https://tvoje-korisnicko-ime.github.io/magnet-metod/`

   To je sada tvoj živi sajt.

## Kad budeš imao svoj domen

Kada kupiš domen (npr. `magnetmetod.rs`), u istim **Settings → Pages** podešavanjima postoji polje **Custom domain** gde ga upišeš, i GitHub ti daje uputstvo koje DNS zapise treba da dodaš kod registra domena. Javi mi kad dođeš do tog koraka, mogu da ti pomognem i oko toga.

## Ako budeš hteo izmene ubuduće

Slobodno mi vrati fajl (ili traži izmenu ovde) — nastavljamo odatle gde smo stali. Kad budeš zadovoljan finalnom verzijom, samo zameni `index.html` i/ili fajlove u `assets/` u repozitorijumu i sajt će se automatski osvežiti za par minuta.
