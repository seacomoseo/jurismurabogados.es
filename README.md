# jurismurabogados.es

[![jurismurabogados.es](/assets/media/logo.png)](https://jurismurabogados.es/)


## STEPS


### After client validate web


#### Domain

- If Netlify
  - [`Domain Management / settings`](https://app.netlify.com/sites/jurismur/settings/domain)
  - `Add custom domain`
  - `Check DNS configuration` Copy
  - Add `DNS Records` copied from Netlify to Domain gestor:
    - From: `jurismurabogados.es`
      DNS Record: `ALIAS`, `ANAME` or `flattened CNAME`
      To: `apex-loadbalancer.netlify.com`
    - From: `jurismurabogados.es`
      DNS Record: `A`
      To: `75.2.60.5`
    - From: `www`
      DNS Record: `CNAME`
      To: `jurismur.netlify.app.`
    - Maybe you need to eliminate the previous records with similar names
  - `Verify DNS configuration`


#### [Google Search Console](https://search.google.com/search-console)

- Add property
- Verify versions ⏩ `data/config.yml`
  - `google_analytics`
  - `google_site_verification`
  - `google_file_verification`
  - DNS:
    From: `@`
    DNS Record: `TXT`
    To: `google-site-verification=[google_site_verification]`
- Link with Analytics
- Add sitemap.xml


##### Delivery

Send to all collaborators next:

```
*ENTREGA WEB jurismurabogados.es:* https://seacomoseo.com/entrega/
```
