# MIS-SKB

# Supplier Knowledge Base (SKB)

The **S**upplier **K**nowledge **B**ase **(SKB)** is the knowledge database of the **Manufacturer Information Service (MIS)**.

| SKB is still under development. Contributions in form of requirements, issues and pull requests are highly welcome. |
|-----------------------------|

## SKB Overview

The graph-based **Supplier Knowledge Base** consists of manufacturing capability information and related data. 
It contains and links this information within interlinked semantically enriched knowledge graphs. 
Since it contains the onboarding data submitted by suppliers and On-Demand Manufacturing (ODM) platforms (via the **Asset Management Service** ), it provides the data basis for matchmaking between offered and required manufacturing capabilities. 
To achieve this, the **Supplier Knowledge Base** contains several AI modules for semantic integration and automated linking to autocomplete the graphs.

The graph-based **Supplier Knowledge Base** uses the following ontology: :blue_book: [Ontology Spec](https://www.smartfactoryweb.de/docs/models/SFW_Ontology_Spec_1.0.pdf) and further information [here](https://eclipse-tractusx.github.io/docs-kits/kits/Manufacturing%20as%20a%20Service%20Kit/Software%20Development%20View/Architecture%20Manufacturing%20as%20a%20Service%20Kit#531-supplier-knowledge-base)

Classification of the SKB based on the MIS architecture.

![SKB](/../main/docs/src/images/SKB.PNG)


The following use cases can be performed with the SKB.

### Indirect Use Cases of the SKB
> [!NOTE]
> Indirect use of the SKB via other MIS components
1. UC1 **Manual onboarding**
- Onboarding of manufacturer information via factory connectors.
- AI-based onboarding of manufacturer information, based on machine specifications.
2. UC2 **Automatic onboarding / crawling**
- The manufacturers' production capabilities are automatically read out by querying the factory connectors.
3. UC3 **Requesting manufacturer information**
- Data consumer can use the MIS to query information such as production capabilities for a data provider.
4. UC4 **Search for potential suppliers/supply chains**
- Identification of potential suppliers/supply chains for a given production process.

### Link to the other MIS components

| Components    | Goals         | URL           |
| ------------- | ------------- | ------------- |
| **Supplier Knowledge Base (SKB)** | Knowledge base for manufacturer/supplier information including capabilities, properties, etc. | [MIS-SKB](https://github.com/FraunhoferIOSB/MIS-SKB)  |
| **Asset Management and Refinement Application (AMARA)**  | Automatically derives manufacturing capabilities from machine specifications with Large Language Models (LLM)  | [MIS-AMARA](https://github.com/FraunhoferIOSB/MIS-AMARA) |
| **Asset Management Service (AMS)**  | Interface to manage asset information like enterprise, factories, manufacturing capabilities, etc. within the knowledge base |[MIS-AMS](https://github.com/FraunhoferIOSB/MIS-AMS)  |
| **Search Engine (SE)**  | Provision of manufacturer information such as production capabilities for a given process description  | [MIS-SE](https://github.com/FraunhoferIOSB/MIS-SE)  |
