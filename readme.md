# Annotating the Seefeld region website

* Organziation: The Seefeld DMO [**Oleksandra**]
* ... [**Umut**]
* TouristInformationCenter: The tourist information centers of Seefeld, Scharnitz, Leutasch, Mösern and Rinn [**Elias**]

Seefeld Website: `http://www.seefeld.com/`

## Seefeld DMO

## ???

## TouristInformationCenter
The website of the TouristInformationCenter is `http://www.seefeld.com/tirol-service/tourist-info`. The five different **tourist information centers** are **organizations** and should be packed into an array of organizations as **subOrganizations** of the DMO organization annotation.

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
