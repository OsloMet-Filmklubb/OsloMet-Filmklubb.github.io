---
# --- FRONT MATTER TEMPLATE FOR FILMVISNING ---
draft: true                    # sett til false når du vil publisere

title: "" # vanligvis navnet på filmen med årstall. Eks: "The Lighthouse (2019)"
date: {{ .Date }}              # Dato for visning
publishDate: {{ .Date }}       # Når innlegget blir synlig på siden
expiryDate: {{ .Date }}        # Når innlegget automatisk skjules (sett gjerne til dagen etter visning)
cover: ""                      # liggende bilde, gjerne fra themoviedb.org (brukes i lister og previews)
summary: ""                    # Kort introduksjon, 1–2 setninger
author: ""                     # Filmens tagline / sitat
tags:                          # Metadata for søk og filtrering
  - Sjanger1
  - Sjanger2
  - Sjanger3
  - Regissør
  - Hovedskuespiller1
  - Hovedskuespiller2
  - Hovedskuespiller3

# --- VISNINGSINFO ---
klokkeslett: "00:00"           # Eks. "16:30"
sted: "Lille Auditorium, P32"  # Visningssted

# --- FILMINFO ---
filmtittel: ""                 # Navn på filmen uten årstall
utslippsår: 0                  # Eks. 2019
spilletid: 0                   # I minutter
aldersgrense: 0                # 0 = Alle
filmbeskrivelse: ""            # Ca ett avsnitt, bruk markdown. Unngå spoilers.
plakat: ""                     # Lenke til original plakat (stående bilde, gjerne fra themoviedb.org)
---
## Visningsinformasjon
**Tid:**            {{< dateformat >}} - {{< param "klokkeslett" "Ukjent" >}}  
**Sted:**           {{< param "sted" "Ukjent" >}}  


## Om Filmen:  
**Tittel:**      {{< param "filmtittel" "Ukjent" >}}   
**Utslippsår:**      {{< param "utslippsår" "Ukjent" >}}  
**Spilletid:**      {{< param "spilletid" "Ukjent" >}} min   
**Aldersgrense:**   {{< param "aldersgrense" "Alle" >}}

{{< markdownParam "filmbeskrivelse" >}}

![Plakat for {{< param "filmtittel" "Ukjent" >}}]({{< param "plakat" "Ukjent" >}})
*{{< param "filmtittel" "Ukjent" >}} ({{< param "utslippsår" "Ukjent" >}}) [kilde]({{< param "plakat" "Ukjent" >}})* 

