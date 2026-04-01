# Shodan

## Link
https://www.shodan.io

---

## What It Does
Shodan is a search engine for internet-connected devices and services. Instead of searching webpages like Google, it searches servers, cameras, routers, industrial systems, websites, and exposed ports.

---

## Why It Matters
Shodan is useful for passive reconnaissance because it helps identify what systems are visible from the internet and what services they appear to be running.

---

## Key Search Filters

- `port:80`  
  Search by port number

- `country:US`  
  Search by country

- `org:"Organization Name"`  
  Search by organization

- `hostname:example.com`  
  Search by hostname

- `product:Apache`  
  Search by software or product

---

## Step-by-Step Example 1: Search for a Company Domain

### Goal
See whether Shodan has indexed internet-facing assets related to a domain.

### Query
hostname:example.com

### Steps
1. Open Shodan
2. Search `hostname:example.com`
3. Review the returned hosts
4. Look for:
   - IP addresses
   - open ports
   - service banners
   - hosting providers
5. Document the visible infrastructure

### Why This Helps
This gives a high-level view of what internet-facing assets may exist.

---

## Step-by-Step Example 2: Find a Specific Service

### Goal
Search for systems running a specific service.

### Query
nginx port:443 country:US

### Steps
1. Open Shodan
2. Search `nginx port:443 country:US`
3. Narrow results further if needed by adding:
   - `org:"Company Name"`
   - `hostname:example.com`
4. Review banners and metadata
5. Note the versions, service types, and exposure

### Why This Helps
This can reveal what technologies are exposed and how common certain services are.

---

## Step-by-Step Example 3: Passive Recon on an Organization

### Goal
Identify what services appear exposed for a known organization.

### Query
org:"Target Organization"

### Steps
1. Search `org:"Target Organization"`
2. Review assets returned under that organization
3. Look for:
   - web servers
   - VPN portals
   - remote access services
   - unusual or outdated systems
4. Record what appears relevant without interacting with any system

### Why This Helps
This helps build an infrastructure profile from passive data.

---

## Use Cases

- Discovering internet-facing assets
- Identifying exposed services
- Understanding technology stacks
- Supporting early-stage reconnaissance

---

## Important Notes

- Shodan is passive because it shows indexed results
- Do not attempt unauthorized access to anything you find
- Service banners may be outdated, so verify carefully
- Best used with other tools such as Google Dorking and passive domain research
