---
uid: KI_Unable_to_open_trended_parameter_cards_via_Cube_advanced_search
---

# Unable to open trended parameter cards via Cube advanced search

## Affected versions

From DataMiner Cube 10.4.0 [CU12]/10.5.0/10.5.3 onwards.

## Cause

To facilitate communication between different modules, a serializable `DataObject` is used to create instances from a string, relying on reflection. Because of an issue introduced in DataMiner 10.4.0 [CU12]/10.5.0/10.5.3 (RN 42552), the reflection process for parameters is broken, preventing the correct `MethodInfo` from being located. As a result, parameter cards cannot be opened directly via navigation in Cube.

## Fix

No fix is available yet.

## Workaround

To access a trended parameter card, follow these steps:

1. In the Surveyor, click the element associated with the parameter.

1. On the element's Data Display page, double-click the trended parameter to open its parameter card.

## Description

In Cube's Advanced Search module, selecting a trended parameter from the search results no longer opens the corresponding parameter card.
