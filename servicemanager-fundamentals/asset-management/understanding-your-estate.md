# Understanding Your Estate

## One view across multiple repositories

Where different parts of your organization need their own segregated set of assets - by business unit, region, or security requirement - Hornbill's asset partitions let you split your register into access-controlled groups, each with its own permissions, while still giving appropriately privileged users a single consolidated view across all assets and partitions.

**Learn more:** [Assets Overview](/servicemanager-config/assets/manage-partitions)

## How assets relate to partitions, sites, departments, and people

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'lineColor': '#808080', 'textColor': '#404040', 'edgeLabelBackground': '#ffffff', 'clusterBkg': '#C0C0C0', 'clusterBorder': '#808080', 'titleColor': '#404040', 'fontSize': '14px'}}}%%
flowchart TB
    classDef org fill:#0C4C8C,stroke:#85D2FF,color:#ffffff
    classDef asset fill:#0065CB,stroke:#85D2FF,color:#ffffff
    classDef support fill:#404040,stroke:#A0A0A0,color:#ffffff

    subgraph ORG["Organization structure"]
        CO["Company"] --> DIV["Division"] --> DEP["Department"]
    end

    SITE["Site<br/>physical location"]
    PEOPLE["People<br/>co-workers and contacts"]
    PART["Partition<br/>or Un-partitioned assets"]
    ASSET["Asset record"]
    AGENTS["Agents<br/>access granted by user or role"]

    CO -. "associated with" .-> SITE
    DEP -- "has members" --> PEOPLE
    PEOPLE -- "based at one site" --> SITE
    DEP -. "can be segregated by" .-> PART
    PART -- "holds each asset in<br/>exactly one partition" --> ASSET
    ASSET -- "Department" --> DEP
    ASSET -- "Site" --> SITE
    ASSET -- "Owned by" --> PEOPLE
    ASSET -- "Used by or Shared with" --> PEOPLE
    AGENTS -- "view, create, update, delete" --> PART

    class CO,DIV,DEP org
    class PART,ASSET asset
    class SITE,PEOPLE,AGENTS support
```

- **Partitions** control who can see and manage an asset. Every asset sits in exactly one partition, or in the Un-partitioned container, and agents are given access to a partition by user or role.
- **Sites** record where an asset physically is. Sites can be associated with a company in your organization structure, and each person is based at one site.
- **People** are linked to an asset as its owner, and as either its single primary user (*Used by*) or one of several users it is *Shared with*.
- **Departments** are groups of the *Department* type in your organization structure. An asset's *Department* field links it directly to one of these groups, and the people in the department are members of the same group. Where a department's assets need to be kept separate, you can give that department its own partition.

**Learn more:** [Asset Details](/servicemanager-user-guide/asset-management/asset-details) | [Locations](/esp-config/organizational-data/locations) | [Groups and Teams](/esp-config/organizational-data/organization)

## Defining your authorized asset portfolio

Because every asset must be created against a defined asset type, and asset types are themselves configured and controlled by administrators, your asset type list effectively defines the portfolio of authorized, supported IT assets for your organization. Assets discovered or imported that don't match an authorized type or model can be surfaced through Hornbill's reporting to help identify unauthorized or unsupported items.

**Learn more:** [Manage Asset Types](/servicemanager-config/assets/asset-types-overview)
