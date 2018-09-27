---
abstract: Component for storing and serving 'cases' compliant with the GEMMA RGBZ, RSGB and ImZTC standards.
tags: hlm
hlmLayers: 4 5
---

# Zaakregistratiecomponent

This component provides the service for storing, managing and sharing cases as used in case management. It is the backbone of the 'case based working methodology' and provides the infrastructure for working with internal and external stakeholders to resolve cases well and within the right timeframe.

This component provides an API to manage it and a rudimentary web interface for viewing the raw data.

Implementation of the referececomponent 'Zaaksysteem' according to the GEMMA Standaard Zaak- en Documentservices (ZDS) 1.2. This component is meant to work together with the [Documentregistratiecomponent](documentregistratiecomponent.md) for storing documents related to the case and with the [Zaaktypecataloguscomponent](zaaktypecatalogus.md) that manages the schema of the types of 'cases' that can be stored.

For more information on the component, used standards and how to implement it go to [GitHub: Haarlem/zaakregistratiecomponent](https://github.com/Haarlem/zaakregistratiecomponent)
