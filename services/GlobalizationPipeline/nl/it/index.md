---

copyright:
  years: 2015, 2016

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}


# Introduzione alla {{site.data.keyword.GlobalizationPipeline_full}}
{: #globalizationpipeline}

*Ultimo aggiornamento: 6 luglio 2016*
{: .last-updated}

{{site.data.keyword.GlobalizationPipeline_full}} è un servizio che fornisce le funzionalità di machine translation e modifica per una rapida traduzione del web o delle IU mobili. Con il relativo dashboard, l'API RESTful e l'integrazione con la delivery pipeline della tua applicazione, puoi distribuire ai clienti globali senza ricreare o ridistribuire la tua applicazione.
{:shortdesc}

Puoi utilizzare il servizio {{site.data.keyword.GlobalizationPipeline_full}} con qualsiasi applicazione in {{site.data.keyword.Bluemix}} o senza binding da sola. Puoi creare, mantenere e rivedere le traduzioni rapidamente, con sforzo minimo a senza dover lasciare il tuo ambiente DevOps.

Dall'interfaccia {{site.data.keyword.GlobalizationPipeline_full}}, puoi tradurre velocemente le tue applicazioni {{site.data.keyword.Bluemix_notm}}. Per informazioni sulla traduzione utilizzando l'API RESTful, consulta [API Reference](https://gp-rest.ng.bluemix.net/translate/swagger/index.html){: new_window}. 


## Creazione di un bundle
{: #globalizationpipeline_creatingbundles}

Con il servizio {{site.data.keyword.GlobalizationPipeline_full}}, puoi creare bundle, che includono i file di risorsa delle tue applicazioni che saranno tradotti. I file di risorsa possono essere file Java Properties, AMD I18N o JSON e devono avere il contenuto nel formato di coppie chiave/valore che rappresentano le stringhe IU dalla tua applicazione.  Per ulteriori dettagli e esempi di tipi di file supportati, consulta [Gestione dei bundle](./bundles.html){: new_window}.

Per creare un bundle, completa la seguente procedura:

1\. Dalla scheda **Overview**, fai clic su **New Bundle**.

2\. Fornisci informazioni sul tuo bundle:

| Campo | Obbligatorio| Descrizione |
|-------|---------|------------|
| **ID Bundle** | Sì | Un nome univoco per identificare il bundle. |
| **Lingua di origine** | Sì | La lingua nativa del file di origine. |
| **File di risorsa** | No | Un [file di risorsa](bundles.html#globalizationpipeline_workingwithbundles) da tradurre. La dimensione massima del file è limitata a 2MB. I file di risorsa specificati saranno caricati.  |
| **Formato file** | No | Il tipo di file che sta venendo caricato. |
| **Lingua di destinazione** | No | Le lingue di cui si desidera la traduzione. |

**Nota:** per modificare il servizio della lingua che fornisce la machine translation per i tuoi bundle, fai clic sulla scheda [**MT Configuration**](./managing_translations.html#globalizationpipeline_service_to_service) per visualizzare gli altri motori machine translation supportati.

3\. Fai clic su **Save**

Dopo che è stato creato il bundle, il file di risorsa caricato viene tradotto nelle lingue di destinazione che hai specificato. Il nuovo bundle viene aggiunto alla scheda Bundles dove puoi:

* Aggiungere o rimuovere le lingue
* Modificare le traduzioni generate
* Aggiornare il file di origine utilizzato nel bundle e rigenerare le traduzioni.

## Importazione dei bundle tradotti nel servizio
{: #globalizationpipeline_importtranslatedbundlesintoservice}

In alternativa, se già disponi di file di risorsa tradotti, puoi importarli in un nuovo bundle. Per ulteriori informazioni, consulta [Java Client Tools for {{site.data.keyword.GlobalizationPipeline_full}}](https://github.com/IBM-Bluemix/gp-java-tools).

**Nota:** se il file di origine iniziale viene aggiornato, le chiavi e i valori definiti nel file vengono sincronizzati con la versione più recente del file di origine in modo che vengano tradotti solo i valori e la chiavi modificati.

## Stima dell'utilizzo dati della {{site.data.keyword.GlobalizationPipeline_full}}
{: #globalizationpipeline_documentpricing}

{{site.data.keyword.GlobalizationPipeline_full}} memorizza le tue traduzioni in un database di backend. Per stimare la dimensione dei dati attivi, puoi fare riferimento alla seguente formula:

`<expected resource data storage size in MB> ˜= 0.0005 * <number of key/value pairs in the source resource> * <number of languages including the source language>`

In basa alla formula, la dimensione di un bundle tipico è `(length of key + length of value in UTF-8 = ˜40 bytes)`.

Ad esempio, se hai 100 coppie chiave/valore e le hai tradotte in 9 lingue, la dimensione di memorizzazione stimata è 0.0005 100 (9+1) = 0.5 MB. La dimensione attuale può essere differente a seconda della dimensione chiave/valore attuale e ai metadati archiviati con la traduzione.

Utilizza il Calcolatore prezzi Bluemix [](https://console.ng.bluemix.net/?direct=classic/#/pricing/cloudOEPaneId=pricing&paneId=pricingSheet&orgGuid=127a45f4-4461-4d5b-a26b-6dc2fdd1a3a2&spaceGuid=208fb1ff-413b-4fd9-9615-e8226062d0f3) per determinare i tuoi costi del servizio mensili.


# Link correlati 
{: #rellinks}
## Esercitazioni ed esempi
{: #samples}

* [Node.js Sample](https://github.com/IBM-Bluemix/gp-nodejs-sample){: new_window}
* [Ruby Sample](https://github.com/IBM-Bluemix/gp-ruby-sample){: new_window}

## SDK
{: #sdk}

* [Java Client](https://github.com/IBM-Bluemix/gp-java-client){: new_window}
* [Java Tools](https://github.com/IBM-Bluemix/gp-java-tools){: new_window}
* [JavaScript Client](https://github.com/IBM-Bluemix/gp-js-client){: new_window}
* [AngularJS Client](https://github.com/IBM-Bluemix/gp-angular-client){: new_window}
* [Ruby Client](https://github.com/IBM-Bluemix/gp-ruby-client){: new_window}
* [Python Client](https://github.com/IBM-Bluemix/gp-python-client){: new_window}

## Riferimento API 
{: #api}

* [IBM Globalization Pipeline RESTful API](https://gp-rest.ng.bluemix.net/translate/swagger/index.html){: new_window}

## Link correlati 
{: #general}

* [Integrate Globalization Pipeline with Delivery Pipeline](https://hub.jazz.net/docs/deploy_ext/#globalize){: new_window}
* [IBM Bluemix Pricing Sheet](https://www.ng.bluemix.net/#/pricing){: new_window}
* [IBM Bluemix Prerequisites](https://developer.ibm.com/bluemix/support/#prereqs){: new_window}
