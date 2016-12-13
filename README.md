# Annotating the Seefeld region website

* Organization: The Seefeld DMO [**Oleksandra**]
* Website [**Umut**]
* TouristInformationCenter: The tourist information centers of Seefeld, Scharnitz, Leutasch, Mösern and Rinn [**Elias**]

Seefeld Website: `http://www.seefeld.com/`

## Seefeld DMO
Oleksandras description here!

## Seefeld.com Web Site
The annotation of **WebSite** http://seefeld.com. This annotation may be connected to the **Organization** and **TouristInformationCenter** annotations. For instance, the source code of the web site contains OpenGraphProtocol tags describing the publisher of the website which is *Informationsbüro Seefeld*.
### Properties used
* url
* image (meta)
* name (meta title)
* headline (experimental)
* description (meta)
* publisher (meta)
* keywords (meta)
* spatialCoverage
* contributor
* copyrightHolder
* copyrightYear
* creator
* inLanguage
* isAccessibleForFree
* mainEntity
* potentialAction (annotated as the google's example suggested. not entirely correct annotation)

### Other properties may be relevant
* accessibilityAPI
* accessibilityControl
* accessibilityFeature
* accesibilityHazard
* accountablePerson
* aggregateRating
* audience
* award
* comment
* commentCount
* dateCreated
* dateModified
* datePublished
* license
* review
* translator
* video
* image
* sameAs

## TouristInformationCenter
The webpage of the TouristInformationCenter is `http://www.seefeld.com/tirol-service/tourist-info`. The five different **tourist information centers** are **organizations** and should be packed into an array of organizations as **subOrganizations** of the DMO organization annotation.

```javascript
{
    "@context": "http://schema.org/",
    "@type": "Organization",
    "name": "Seefeld Tourismus",
    ...,

    "subOrganization": [
      {
        Seefeld content
      },
      {
        Scharnitz content
      },
      {
        ...
      },
      ...
    ]
}
```
