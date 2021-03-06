---
description: "[One paragraph description]\n[References to supporting information like\
  \ \u201Cuse cases\u201D, \u201Cbioschemas mapping\u201D and \u201Cschema.org posted\
  \ issues\u201D]\n"
edit_url: https://github.com/BioSchemas/bioschemas.github.io/edit/master/_newSpecs/Tool.md
extended_props:
  CreativeWork:
  - bsc_dec: ''
    cardinality: ONE
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - Person
    marginality: Minimum
    name: accountablePerson
    sdo_desc: Specifies the Person that is legally accountable for the CreativeWork.
  - bsc_dec: ''
    cardinality: MANY
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - CreativeWork
    - Text
    marginality: Minimum
    name: citation
    sdo_desc: A citation or reference to another creative work, such as another publication,
      web page, scholarly article, etc.
  - bsc_dec: publication, publication/doi
    cardinality: MANY
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - PublicationEvent
    marginality: Recommended
    name: publication
    sdo_desc: A publication event associated with the item.
  SoftwareApplication:
  - bsc_dec: ''
    cardinality: MANY
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - Text
    - URL
    marginality: Minimum
    name: featureList
    sdo_desc: Features or modules provided by this application (and possibly required
      by other applications).
  - bsc_dec: softwareHelp:url, softwareHelp:genre, softwareHelp:description/review
    cardinality: MANY
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - CreativeWork
    marginality: Minimum
    name: softwareHelp
    sdo_desc: Software application help.
  - bsc_dec: contact/email, contact/url, contact/name, contact/tel, contact/type
    cardinality: MANY
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - Text
    - URL
    marginality: Minimum
    name: softwareRequirements
    sdo_desc: 'Component dependency requirements for application. This includes runtime
      environments and shared libraries that are not included in the application distribution
      package, but required to run the application (Examples: DirectX, Java or .NET
      runtime).'
  - bsc_dec: ''
    cardinality: ONE
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - DataFeed
    marginality: Minimum
    name: supportingData
    sdo_desc: Supporting data for a SoftwareApplication.
  Thing:
  - bsc_dec: ''
    cardinality: MANY
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - Text
    marginality: Minimum
    name: description
    sdo_desc: A description of the item.
  - bsc_dec: ''
    cardinality: MANY
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - Text
    marginality: Optional
    name: name
    sdo_desc: The name of the item.
g_mapping_file: Tool Mapping
gh_folder: https://github.com/BioSchemas/Tool
gh_tasks: https://github.com/BioSchemas/bioschemas/labels/type%3A%20Tool
hierarchy:
- SoftwareApplication
- CreativeWork
- Thing
layout: new_spec_detail
name: Tool
new_props: []
parent_type: SoftwareApplication
spec_mapping_url: https://docs.google.com/spreadsheets/d/1D0aQl-Ocp8Fi7a-drKV1Faed6tYUgGwzEM8xypa8S2Y/edit?usp=drivesdk
spec_type: Profile
status: revision
subtitle: Bioschemas specification for describing SoftwareApplication in the life-science.
version: 0.0.1
---