# VUE.JS

## Introduzione
- Rendering dichiarativo : Vue estende l'HTML standard con una sintassi del modello che ci consente di descrivere in modo dichiarativo l'output HTML in base allo stato JavaScript.

- Reattività : Vue tiene traccia automaticamente delle modifiche allo stato di JavaScript e aggiorna in modo efficiente il DOM quando si verificano modifiche.

#### Vue può essere utilizzato in diversi modi:
- Miglioramento dell'HTML statico senza una fase di creazione
- Incorporamento come componenti Web in qualsiasi pagina
- Applicazione a pagina singola (SPA)
- Full Stack/Rendering lato server (SSR)
- Jamstack/Generazione di siti statici (SSG)
- Targeting per desktop, dispositivi mobili, WebGL e persino terminale

#### Componenti a file singolo​
Nella maggior parte dei progetti Vue abilitati per lo strumento di creazione, creiamo componenti Vue utilizzando un formato di file simile a HTML chiamato componente a file singolo. Incapsula la logica del componente (JavaScript), il modello (HTML) e gli stili (CSS) in un unico file.

## Sintassi

#### Interpolazione del testo
La forma più elementare di associazione dati è l'interpolazione del testo utilizzando la sintassi doppie parentesi graffe:

<code> Message: {{ msg }} </code>

Il tag <code>msg</code> verrà sostituito con il valore della msg proprietà dell'istanza del componente corrispondente . Verrà inoltre aggiornato ogni volta che la msg proprietà cambia.

## HTML grezzo

Doppi baffi interpretano i dati come testo semplice, non HTML. Per produrre HTML reale, dovrai utilizzare la <code>v-html</code> direttiva

L' v-html attributo è chiamato direttiva . Le direttive hanno il prefisso v-per indicare che sono attributi speciali forniti da Vue e, come avrai intuito, applicano un comportamento reattivo speciale al DOM renderizzato.

I baffi non possono essere utilizzati all'interno degli attributi HTML. Utilizzare invece una v-binddirettiva, la v-binddirettiva indica a Vue di mantenere l'attributo dell'elemento con la proprietà del componente.

Poiché v-bindè così comunemente usato, ha una sintassi abbreviata dedicata <code>:id="dynamicid"</code>