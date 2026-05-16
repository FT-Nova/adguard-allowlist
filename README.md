# AdGuard Allowlist

Custom allowlist for AdGuard DNS / AdGuard Home.  
Add domains here that should **not** be blocked.

## Format

Use [AdGuard DNS filtering syntax](https://adguard-dns.io/kb/general/dns-filtering-syntax/):

```
! Comment lines start with ! or #
@@||domain.tld^    → unblock domain + all subdomains (recommended)
@@domain.tld       → unblock exact domain only
domain.tld         → domains-only syntax (unblocks domain + subdomains)
```

**Examples:**

```
@@||derstandard.at^
@@||orf.at^
@@||reddit.com^
```

## Usage

1. Go to your AdGuard Home / AdGuard DNS settings
2. Add a **DNS allowlist** pointing to the raw file:
   `https://raw.githubusercontent.com/FT-Nova/adguard-allowlist/main/allowlist.txt`
3. Or just copy the entries manually into your custom filtering rules

## Entries

See [`allowlist.txt`](./allowlist.txt).
