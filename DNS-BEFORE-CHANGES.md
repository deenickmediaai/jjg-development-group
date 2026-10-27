# jjgdevelopmentgroup.com DNS, recorded before pointing the domain at Vercel

Captured 2026-10-27 from Google Public DNS. Registrar/DNS host: GoDaddy
(nameservers ns35/ns36.domaincontrol.com).

## Rows that CHANGE to point the site at Vercel

| Type  | Name | Current value                       |
|-------|------|-------------------------------------|
| A     | @    | 13.248.243.5                        |
| A     | @    | 76.223.105.230                      |
| CNAME | www  | jjgdevelopmentgroup.com             |

The two A records are GoDaddy's parked-page servers (AWS Global Accelerator).

## Rows that MUST NOT be touched: John's email

John's mail is Microsoft 365 filtered through Proofpoint Essentials. Changing
or deleting any of these stops him receiving email.

| Type  | Name          | Value                                                                |
|-------|---------------|----------------------------------------------------------------------|
| MX    | @ (prio 0)    | mx1-usg2.ppe-hosted.com                                              |
| MX    | @ (prio 0)    | mx2-usg2.ppe-hosted.com                                              |
| MX    | @ (prio 0)    | mx3-usg2.ppe-hosted.com                                              |
| TXT   | @             | NETORG20322567.onmicrosoft.com                                       |
| TXT   | @             | v=spf1 include:_spf-usg2.ppe-hosted.com include:secureserver.net ~all |
| CNAME | autodiscover  | autodiscover.outlook.com                                             |

The onmicrosoft TXT proves domain ownership to Microsoft 365. The SPF record
tells other mail servers which servers may send as this domain; deleting it
sends John's outgoing mail to spam. Autodiscover is what configures Outlook.

## To restore

Put the A and CNAME rows in the first table back exactly as listed.
