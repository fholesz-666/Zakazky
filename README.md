# Zakázky

Jednoduché webové CRM na zakázky FVE a LPS a obecné úkoly.

- Hosting: GitHub Pages (tato složka, soubor `index.html`)
- Data a přihlašování: Supabase projekt `zakazky-crm`
- Kdokoli si může založit účet a dostane vlastní prostor „Moje úkoly“.
- Prostor „FVE a LPS“ patří účtu fholesz@gmail.com, ten do něj přidává další lidi v Nastavení.
- Kalendář: každý prostor má vlastní odkaz pro odběr v Apple Kalendáři (Kalendář → Odběr).

## Supabase
- Tabulky: `workspaces`, `workspace_members`, `jobs` (data zakázky v JSON), přístup hlídá RLS.
- Edge funkce `accounts` (registrace bez potvrzovacího e-mailu) a `ics` (kalendářový odběr).
