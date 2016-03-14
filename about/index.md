---
layout: page
title: About
---

BuildingSync<sup>&reg;</sup> is a standardized language for commercial building energy audit data that software developers can use to exchange data between audit tools. Taking the form of an [XML schema](https://en.wikipedia.org/wiki/XML_Schema_(W3C)), BuildingSync can be required by building owners and audit program managers to allow data analysis and aggregation across multiple buildings in order to evaluate program performance and analyze trends.

BuildingSync was developed using the standard energy data terminology defined in the [Building Energy Data Exchange Specification (BEDES)](https://bedes.lbl.gov/). BuildingSync is one of the first implementations of BEDES Version 1.0, and it was developed in close collaboration with the BEDES working groups.

{% comment %}
Graphic illustrating above text, possibly the same one on the main page
{% endcomment %}

BuildingSync standardizes the format of the energy audit data itself.  It is not intended to standardize the calculations performed on these data by engineers, analysts, software packages, or other audit tools.

BuildingSync consists of two files and a reference sheet, which are all offered as [free downloads](https://github.com/BuildingSync/schema/releases):

- The data field "dictionary" {% comment %}TODO: hyperlink to download location{% endcomment %} in Excel format, including field names, definitions, units, and other attributes. The data dictionary is aligned with BEDES, but includes only the subset of data fields that are relevant for energy audits. This file can be referenced to help standardize the terminology used in energy audits, but does it does not provide a structure that allows data to be exchanged across different applications.
- An XML Schema file (.xsd) {% comment %}TODO: hyperlink to download location{% endcomment %} that documents the relationships among the data fields. This file can be referenced as a voluntary or mandatory reporting format for audit data, and data files compliant with the schema can then be aggregated and analyzed in a database. There are several tools available for viewing a graphical version of the XML schema file. View the [Wikipedia page about XML schema editors](https://en.wikipedia.org/wiki/XML_Schema_Editor#XML_Schema_Editors) for more information about XML viewers.
- The BuildingSync Geometry Reference Sheet {% comment %}TODO: hyperlink to download location{% endcomment %}, which illustrates how most of the simplified geometric terms (shapes, side names, vertices, orientations) are defined in the context of BuildingSync.

##### Why was BuildingSync developed?
Currently the energy audit industry lacks a common data collection format. Data collection differs widely between energy auditors, as do the outputs from various energy audit software tools. This makes it difficult to aggregate the data collected by different auditors, or to make comparisons between buildings that have been audited by different auditors using different software.

Energy audits of commercial buildings are becoming increasingly common, and even required, in the federal sector and in cities like New York City and San Francisco. The [American Society of Heating, Refrigeration and Air Conditioning Engineers (ASHRAE)](https://www.ashrae.org/) is in the process of developing a national standard for commercial building energy audits; however, this process is complicated by the lack of a standard data specification for information collected and reported, as well as the lack of consistency in data formats across audit software applications.

##### What can BuildingSync do?
BuildingSync can facilitate a consistent history of energy audit data across the life of a building or a group of buildings, and thus enable lower costs and higher energy performance results. It can also allow easier aggregation and analysis of audits conducted by different companies using different software. BuildingSync covers the essential data collected across all ASHRAE Audit Levels as defined in Procedures for Commercial Building Energy Audits, and includes all data necessary for the calculation of a [Commercial Building Energy Asset Score](http://energy.gov/eere/buildings/commercial-building-energy-asset-score).

BuildingSync provides a common schema for energy audit data that can be utilized by a variety of software and databases. Using the schema ensures that data collected for a single building over time is consistent and comparable, that data from different buildings can be easily aggregated and compared for large-scale analysis, and that data can be transferred between a variety of software tools. This streamlines the energy audit process and lead to new opportunities for using the resulting data to achieve greater energy efficiency.

By delivering energy audit data in a common format, energy auditors can make it easier for their customers to use the data to make decisions.  For large building owners with many properties, standardized data across their buildings can help them more easily understand their opportunities for energy efficiency. Standardized data can also make it much easier for building owners to integrate the information they receive in an energy audit into property management tools for later reference and reuse.  Utilities or local governments that run energy audit programs may also find it easier to utilize the results of energy audits to spur energy efficiency improvements if those results are in a common format.

The schema was built using the standard terminology defined in the Building Energy Data Exchange Specification (BEDES) dictionary. Existing data formats and guidance about how to conduct energy audits were incorporated whenever possible, making it easier to reconcile and map data from existing databases to BuildingSync.

{% comment %}
This section will need a graphic, I think.
{% endcomment %}

##### Who should use BuildingSync?
BuildingSync considers the needs and interests of all stakeholders in the energy audit industry, including building owners, auditors, software developers, and program managers. Existing data formats and datasets were leveraged whenever possible, to avoid duplication of effort and minimize the effort required to perform data reconciliation and mapping from existing databases. Using BuildingSync, audit data can be collected and reported in a format that allows many different users to analyze and process the data to answer their specific questions.

- **Providers of building energy assessment software** can integrate the ability to export BuildingSync-compatible files into their software.
- **Providers of energy auditing services** can choose to use software that can output BuildingSync-compatible files.
- **Building owners** may wish to incorporate BuildingSync into their next RFP for a building energy audit by requiring the auditor to provide data in a BuildingSync-compatible format.
- **Utilities** can choose to recommend or require software that uses BuildingSync-compatible files for any programs involving energy audits.
