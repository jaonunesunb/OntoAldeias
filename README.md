# OntoAldeias

OntoAldeias is an application ontology developed to support the dynamic generation of village registration forms in OntoForms, with a focus on standardizing data needed for information management related to health infrastructure projects in Indigenous contexts.

The ontology was modeled in OWL using Protégé and reuses entities from the Basic Formal Ontology (BFO), the Information Artifact Ontology (IAO), the Relation Ontology (RO), and annotation properties from Dublin Core.

## Purpose

OntoAldeias does not aim to represent Indigenous communities in their entirety. Its scope is restricted to the informational structure required to support the generation of registration forms in OntoForms.

The ontology formalizes forms, input fields, restrictions, input types, metadata, and controlled values used in the registration of villages for the context of health infrastructure projects.

## Version

- Ontology name: OntoAldeias
- Version: 1.1.0
- Language: OWL
- Editor: Protégé
- Ontology URI: `http://www.semanticweb.org/ontologias/ontoAldeias`
- Entity namespace: `http://www.semanticweb.org/ontologias/SESAI/`
- Identifier pattern: `ontoAldeias_00000000`

## Scope

OntoAldeias represents the informational structure of village registration forms, including:

- forms;
- input fields;
- input types;
- relations between forms and fields;
- presentation metadata;
- controlled values associated with villages, DSEI, base poles, municipalities, federative units, and Indigenous lands.

## Limitations

OntoAldeias does not model:

- Indigenous communities in their entirety;
- biomedical or individual health aspects;
- legal processes of territorial demarcation;
- technical engineering details;
- broad sociocultural dimensions of Indigenous peoples.

These topics may be addressed by specific ontologies or future extensions, if required by new application contexts.

## Competency Questions

The ontology was guided by competency questions related to its use in OntoForms:

1. Which fields compose a given form?
2. Which input type should be used for each field?
3. Which fields are mandatory or optional?
4. Which controlled values can be displayed in selection fields?
5. Which metadata guide the presentation of fields in OntoForms?

## Conceptual Structure

OntoAldeias distinguishes three main elements:

1. **Form**: modeled as a document and as a plan specification, since it guides the filling structure interpreted by OntoForms.
2. **Form filling process**: a planned process in which the user provides values for the fields defined by the form.
3. **Filled village registration document**: the informational result produced after the form is filled.

This distinction separates the structure used to generate the interface from the document produced after data entry.

## Use in OntoForms

In OntoForms, the ontology is consumed to retrieve:

- form subclasses;
- object properties, such as `tem campo`;
- logical restrictions;
- cardinalities;
- data types;
- annotation properties;
- reusable instances as controlled values.

The property `tem campo` is central to interface generation, since it relates a form class to the input fields that must be rendered. Data properties indicate the expected input type, such as short text, long text, boolean, numeric field, or selection field.

## Metadata

OntoAldeias uses Dublin Core properties and specific annotations to support documentation, traceability, and form rendering.

Examples of metadata used in the ontology include:

- `dc:contributor`
- `dc:date`
- `dc:description`
- `rdfs:label`
- `grupo`
- `placeholder`

These annotations record authorship, creation date, conceptual description, readable label, form group, and filling examples.

## Controlled Values

OntoAldeias uses instances as controlled values for selection fields. These values may include:

- villages;
- DSEI;
- base poles;
- municipalities;
- federative units;
- Indigenous lands.

This strategy helps reduce spelling variations, ambiguities, and typing errors during form filling.

## Repository Files

This repository contains:

- `README.md`: documentation of the ontology;
- `OntoAldeias_v1.1.0.owl`: OWL file of the ontology;
- `LICENSE`: license file.

## License

This ontology and its documentation are licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0).

You are free to share and adapt the material, including for commercial purposes, provided that appropriate credit is given.

License: `https://creativecommons.org/licenses/by/4.0/`
