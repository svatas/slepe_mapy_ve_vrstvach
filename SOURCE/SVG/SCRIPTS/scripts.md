# Skripty pro linuxový curl pro stažení SVG vrstev z OSM Boundaries

## Úvod
Na stránce **[OSM Boundaries](https://wambachers-osm.website/boundaries/)** pana Waltera Nordmanna je možné pomocí skriptů generovat SVG vrstvy s hranicemi založenými na OSM.
Pokud budete chtít tyto skripty využít :
* je neprve zapotřebí se na stránce OSM **[zaregistrovat](https://www.openstreetmap.org/user/new)** nebo se příhlásit.
* vybráním nějaké zeměm a kliknutím na tlačítko **Export** ze stránky **[OSM Boundaries](https://wambachers-osm.website/boundaries/)** získáte ukázkový skript včetně tzv. **cliKey** ve tvaru **xxxxxxxx-xxxx-xxxx-xxxx--xxxxxxxxxxxx**.
* ten pak použijte v níže uvedených skriptech.

**Česko**

curl -f -o Czechia_all.zip --url 'https://wambachers-osm.website/boundaries/exportBoundaries?cliVersion=1.0&cliKey=xxxxxxxx-xxxx-xxxx-xxxx--xxxxxxxxxxxx&exportFormat=svg&exportLayout=levels&exportAreas=land&from_AL=2&to_AL=7&union=false&selected=51684'

**Slovensko**

curl -f -o Slovakia_all.zip --url 'https://wambachers-osm.website/boundaries/exportBoundaries?cliVersion=1.0&cliKey=xxxxxxxx-xxxx-xxxx-xxxx--xxxxxxxxxxxx&exportFormat=svg&exportLayout=levels&exportAreas=land&from_AL=2&to_AL=8&union=false&selected=14296'

**Praha**

curl -f -o Prague_all.zip --url 'https://wambachers-osm.website/boundaries/exportBoundaries?cliVersion=1.0&cliKey=xxxxxxxx-xxxx-xxxx-xxxx--xxxxxxxxxxxx&exportFormat=svg&exportLayout=levels&exportAreas=land&from_AL=4&to_AL=10&union=false&selected=435541'

**Česko a jeho sousední státy**

curl -f -o CZ_neighbours.zip --url 'https://wambachers-osm.website/boundaries/exportBoundaries?cliVersion=1.0&cliKey=xxxxxxxx-xxxx-xxxx-xxxx--xxxxxxxxxxxx&exportFormat=svg&exportLayout=levels&exportAreas=land&union=false&selected=14296,1702499,49715,336075,51477,62422,51684,435541,16239,109166'

**Slovensko a jeho sousední státy**

curl -f -o SK_neighbours.zip --url 'https://wambachers-osm.website/boundaries/exportBoundaries?cliVersion=1.0&cliKey=xxxxxxxx-xxxx-xxxx-xxxx--xxxxxxxxxxxx&exportFormat=svg&exportLayout=levels&exportAreas=land&union=false&selected=14296,1702499,49715,336075,51684,435541,16239,109166,21335,37244,60199,421866'
