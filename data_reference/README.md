# Données e-NDP de référence


Données de référence au niveau registre et page ainsi que les ressources et métadonnées associées (liage aux
services Nakala, SIV, DTS, manifeste etc.).

## `endp_registres_metadata.csv` (niveau registre)

Description des champs : 

- `volume.identifier` : Cote du registre

- `volume.startDate` : Date de début du registre (dates extrêmes)

- `volume.endDate` : Date de fin du registre (dates extrêmes)

- `volume.label` : Intitulé du registre provenant des métadonnées Nakala

- `volume.description` : Description du registre provenant des métadonnées Nakala

- `volume.publisher` : Éditeur(s) des registres provenant des métadonnées Nakala

- `volume.language` : Langue(s) des registres provenant des métadonnées Nakala

- `volume.siv_url` : Lien vers la Salle des inventaires virtuelle des AN de la description archivistique du registre

- `volume.nakala_doi` : Identifiant DOI du registre dans Nakala

- `volume.noSketch_volume` : Identifiant du registre dans NoSketch


## `endp_registres_page_metadata.csv` (niveau page)

Description des champs :

- `volume.page.image.nakala.sha1` : Identifiant (sha1) de la page du registre dans Nakala

- `volume.page.label.original` : Label de la page

- `volume.identifier` : Cote du registre d'où provient la page (clé étrangère pour lier `endp_registres_metadata.csv`)

- `volume.page.image.label.tif` : Label de l'image tif de la page

- `volume.page.label.siv` : Label de l'image de la page dans la SIV des AN

- `volume.page.date.fr_full` : Date en langage naturel (fr, mois année) de la page du registre (peut contenir deux mois avec le séparateur "/" et des valeurs "null" pour les pages de référence colorimétrique identifié par le suffixe "REF")

- `volume.page.date.ISO_full` : Date au format ISO (fr, AAAA-MM) de la page du registre (peut contenir deux mois avec le séparateur "/" et des valeurs "null" pour les pages de référence colorimétrique identifié par le suffixe "REF")

- `volume.page.date.year` : Année de la page du registre (peut contenir, des valeurs "null")

- `volume.page.date.fr_month` : Mois en langage naturel (fr, mois) de la page du registre (peut contenir, des valeurs "null" et des valeurs séparés par "-")

- `volume.page.date.ISO_month` : Mois au format ISO (fr, mois) de la page du registre (peut contenir, des valeurs "null" et des valeurs séparés par "/")

- `volume.page.NoSketch.id` : Identifiant du registre d'où provient la page dans NoSketch (paramètre, peut contenir des valeurs "null")

- `volume.page.NoSketch.volume` : Registre d'où provient la page dans NoSketch (paramètre, peut contenir des valeurs "null")

- `volume.page.NoSketch.folio` : Identifiant de la page dans NoSketch (paramètre, peut contenir des valeurs "null")

- `volume.page.NoSketch.date` : Date de la page dans NoSketch (paramètre, peut contenir des valeurs "null")

- `volume.page.siv.sequence_id` : Identifiant de la séquence où se trouve la page dans la SIV des AN (niveau `<c>` en EAD, peut contenir des valeurs "null")

- `volume.page.siv.sequence_url` : Lien vers la séquence où se trouve la page dans la SIV des AN (peut contenir des valeurs "null")

- `volume.page.siv.media_url` : Lien vers l'image de la page dans la SIV des AN (accès au visualiseur, peut contenir des valeurs "null")