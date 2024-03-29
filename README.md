# Stadgar

Detta är D-sektionen inom TLTHs stadgar. Under "Releases" finns alla versioner av stadgarna och om en följer commit-meddelanden finns mer detaljerad historik.

## Användning
All text i repot ska vara skrivet på svenska.

### Efter ett sektionsmöte
* Klona repot. `git clone https://github.com/Dsek-LTH/stadgar`
* Om du redan klonat det till att du är på senaste revisionen. `git checkout master && git pull`
* Skapa en ny branch. `git checkout -b [branchnamn, tex HTM2-2019]`
* För varje motion och proposition:
    * Ändra main.tex på det sätt som krävs för den nya motionen eller propositionen.
    * Efter varje införd ändring skapa en commit med meddelande innehållande mötesförkortningen för mötet som gjorde andra läsningen och ändringen. `git commit -m "[HTM2 2018] Bytte sektionens Hymn"`
    * Om en mer detaljerad beskrivning behövss bör kroppen av commitens meddelande istället användas. `git commit`
* Se till att att mötesnamn och dagens datum står på varje sida i stadgarna högst upp i högra hörnet.
* Pusha upp din branch till Github `git push -u origin [branchnamn, tex HTM2-2019]`
* Öppna en pull request på https://github.com/Dsek-LTH/stadgar/pulls för att få med dina ändringar till huvudbranchen.
* När denna godkänts, skapas en ny release och PDF automatiskt.

### När du vill göra redaktionella ändringar
Redaktionella ändringar ändrar inte betydelsen av stadgarna, utan ändrar enbart läsbarheten eller rättar små uppenbara fel. För att skapa en redaktionell ändring, följ instruktionerna för "Efter ett sektionsmöte" utöver att commit-meddelandet ska inte innehålla en mötesförkortning utan istället [Redaktionella ändringar]. `git commit -m "[Redaktionella ändringar] Fixade stavfel"`. Döp gärna branchen till något i stil med "redaktionellaandringar".

### När du vill ändringar till repot
Ändringar som inte påverkar stadgarna direkt så som ändringar av continuous integration eller README-filen ska inte innehålla en mötesförkortning utan istället [Repoändringar]. `git commit -m "[Repoändringar] Uppdaterade README"`. Döp gärna branchen till något i stil med "repoandringar"

## Historik
Vid höstterminsmöte 1 2017 togs ett beslut att införa historik för sektionens styrdokument. Det togs även ett beslut att ålägga styrelsen att retroaktivt i den mån det går att införa denna historik. Detta påbörjades genom att i början i styrdokumenten fylla i en tabell med: datum, möte som tog beslutet, motion och vad som ändrades i klartext. Detta var inte hållbart i längden och Styrelsen 2019 flyttade hantering av historiken till Github. Den tidigare historiken ligger i en tidigt commit kallad "tidigare historik". De första ändringarna till styrdokumenten Github användes med var besluten från höstterminsmöte 2 2018.
