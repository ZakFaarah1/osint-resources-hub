# Google Dorking

## Link
https://www.exploit-db.com/google-hacking-database

---

## What It Does
Google Dorking uses advanced Google search operators to locate publicly indexed information that may not be easy to find through normal browsing. It is useful in OSINT because it helps uncover documents, exposed directories, login portals, and other publicly accessible resources.

---

## Why It Matters
Google is often the first reconnaissance tool people use, but advanced operators make it far more powerful. With the right query, you can narrow results to a specific domain, file type, title, or keyword and quickly identify useful information.

---

## Basic Search Operators

- `site:example.com`  
  Searches only within a specific website or domain

- `filetype:pdf`  
  Searches for a specific file type

- `intitle:"index of"`  
  Searches for pages with specific words in the title

- `inurl:admin`  
  Searches for URLs containing a specific word

- `"exact phrase"`  
  Searches for an exact phrase

- `-word`  
  Excludes a word from results

---

## Step-by-Step Example 1: Find Public PDFs on a Target Website

### Goal
Find PDF documents on a company website that may contain useful public information.

### Query
site:example.com filetype:pdf

### Steps
1. Open Google
2. Type `site:example.com filetype:pdf`
3. Review results for:
   - employee directories
   - reports
   - presentations
   - manuals
4. Open only documents that are clearly public and relevant
5. Take notes on names, contact details, technologies, or locations mentioned

### Why This Helps
PDFs often contain useful details such as employee names, internal terminology, addresses, and software references.

---

## Step-by-Step Example 2: Find Login Pages

### Goal
Identify public-facing login portals for a domain.

### Query
site:example.com inurl:login OR inurl:portal

### Steps
1. Open Google
2. Search `site:example.com inurl:login OR inurl:portal`
3. Review results for:
   - staff portals
   - client portals
   - admin panels
4. Document the existence of the pages, but do not attempt unauthorized access

### Why This Helps
This can show what systems are exposed publicly and what technologies may be in use.

---

## Step-by-Step Example 3: Find Exposed Directories

### Goal
Locate open directory listings indexed by Google.

### Query
site:example.com intitle:"index of"

### Steps
1. Search `site:example.com intitle:"index of"`
2. Look for directories containing:
   - backups
   - logs
   - documents
   - uploads
3. Record only what is publicly visible and relevant

### Why This Helps
Open directories can reveal file structures, public assets, and accidental exposures.

---

## Use Cases

- Finding public reports and documents
- Locating exposed login pages
- Discovering archived or forgotten content
- Identifying keywords, employee names, and technologies

---

## Notes

- This is a passive technique because it uses search engine results
- Only access publicly available information
- Avoid queries that move from research into misuse
- Best used early in an investigation to build a picture of the target
