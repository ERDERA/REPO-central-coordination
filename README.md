# ERDERA Github central coordination
## Introduction to the ERDERA GitHub Structure and Governance

The ERDERA GitHub organization serves as the backbone for coordinating the digital resources and collaborative efforts of the ERDERA project. Designed to streamline the development, dissemination, and governance of various work packages and deliverables, the GitHub structure integrates multiple repositories and teams tailored to address specific tasks and objectives within the project.

At the core of this structure is the central coordination repository, which acts as the hub for managing the GitHub organization. It ensures collaboration by standardizing processes such as requesting new repositories, forming teams, and managing access rights. The repository also facilitates cloning and adapting resources from the prior EJP RD project, thus ensuring continuity and leveraging past work.
## Governance of Repository Creation

The ERDERA GitHub organization operates under a distributed governance structure, which ensures that responsibilities for repository creation are shared among central coordination, work package leaders (WPL), and task leaders. This decentralized approach facilitates efficient collaboration and ensures that repositories are created in alignment with project needs and objectives.

Roles and Responsibilities for Repository Creation
### Central Coordination Team:
-	Oversees the overall structure and organization of the ERDERA GitHub.
-   Maintains guidelines for repository naming, access control, and usage.
-   Supports repository creation for cross-cutting tasks or central infrastructure needs.
-   Handles special requests, such as cloning repositories from the EJP RD project.
### Work Package Leaders (WPL):
- Authorized to create repositories for their respective work packages.
- Ensure that repositories are aligned with the deliverables and objectives of the work package.
- Responsible for managing access permissions within their work package team.
### Task Leaders:
- Empowered to issue repositories specific to their task needs within a work package.
- Ensure that task-specific repositories are appropriately scoped and structured.
- Coordinate with work package leaders and central coordination to align repository practices.

## ERDERA GitHub Layers

The ERDERA infrastructure is organized into three primary layers to provide clarity and functional separation:
### Layer 1: SharePoint
Serves as a collaborative document management and storage platform, supporting project documentation and file sharing.
### Layer 2: GitHub
The heart of the technical coordination, where repositories for private, public, and semantic artifacts are hosted. This layer supports the development of SPARQL examples, semantic models, and other resources critical to the project.
### Layer 3: Zenodo
Focuses on archiving and disseminating outputs in alignment with FAIR (Findable, Accessible, Interoperable, and Reusable) principles. Zenodo ensures long-term availability and accessibility of project deliverables.

## How to Engage

To promote transparency and collaboration, ERDERA provides simple mechanisms for partners to request new resources or include existing repositories from EJP-RD and other related projects:
	•	New Team Requests: Facilitates the formation of teams with clearly defined access permissions.
	•	New Repository Requests: Allows contributors to propose new repositories for specific tasks or deliverables.
	•	Repository Cloning: Enables the reuse of resources from the EJP RD project to build on prior work.

By leveraging these mechanisms, partners can efficiently create, manage, and access the digital resources needed to drive the ERDERA project forward. The ERDERA GitHub organization is designed to support the collaborative efforts of the project partners and ensure the successful development and dissemination of project deliverables.

## Github coordinators
The following people are the coordinators for this Github repository:
- [Andra Waagmeester (AmsterdamUMC)](https://github.com/andrawaag)
- [Luiz Olavo Bonino da Silva Santos (UTwente)](https://github.com/luizbonino)
- [Mark Hanauer (Orphanet)](https://github.com/orgs/ERDERA/people/Orphanet)
- [Heena Lad](https://github.com/orgs/ERDERA/people/HeenaLad)
- [Ronald Cornet (AmsterdamUMC)](https://github.com/orgs/ERDERA/people/ronaldcornet)

### Forms
- [Request a new team]()
- [Request a new repository](https://github.com/ERDERA/Central-coordination/issues/new?)
- [Request a clone of a repository from the previous EJP RD project](https://github.com/ERDERA/Central-coordination/issues/new?assignees=&labels=&projects=&template=GitHub_Fork_Clone_request.yml&title=%5BRelocate+Repository%5D%3A+%5BSource+Repo+Name%5D)

### Teams
A github team is a group of people that have access to a set of repositories. The teams are used to manage the access to the repositories. The following teams are currently available in the ERDERA github organization: [Teams](https://github.com/orgs/ERDERA/teams)

### Current repositories
```mermaid
graph TD
    subgraph ClusterA [Layer 1: SharePoint]
        SP[(SharePoint)]
    end

    subgraph ClusterB [Layer 2: GitHub]
    direction LR
        EGH[(ERDERA GitHub)] --> PrivR[Private Repositories]
        EGH --> PubR[Public Repositories]  
        PubR --> WP16[Work package 16]
        WP16 --> SE[Semantic artefacts]
        SE --> SPARQLEX[ERDERA SPARQL Examples]
        PrivR --> CC[Central coordination]
        CC --> WPL[Work package leaders]
        CC --> AMC[AmsterdamUMC]
        WPL --> 13.3[Task 13.3]
        WPL --> 14.1[Task 14.1]
        WPL --> 16.5[Task 16.5]
    end

    subgraph ClusterC [Layer 3: Zenodo]
        EZD[(ERDERA Zenodo)]
    end
    
    ClusterA --> |is coordinated through| ClusterB
    ClusterB --> |is archived and diseminated on| ClusterC




```
- To request new teams, please contact anyone from the central coordination team.
- To request a new repository, please use the [Request a new repository](https://github.com/ERDERA/Central-coordination/issues/new?) form

# Private GitHub repositories
## Central coordination
- [Andra Waagmeester (AmsterdamUMC)](https://github.com/andrawaag)
- [Luiz Olavo Bonino da Silva Santos (UTwente)](https://github.com/luizbonino)
- [Mark Hanauer (Orphanet)](https://github.com/orgs/ERDERA/people/Orphanet)
- [Heena Lad](https://github.com/orgs/ERDERA/people/HeenaLad)
- [Ronald Cornet (AmsterdamUMC)](https://github.com/orgs/ERDERA/people/ronaldcornet)

## Work package leaders
#Todo: Add the work package leaders

## AmsterdamUMC
Availability: private
- [Andra Waagmeester (AmsterdamUMC)](https://github.com/andrawaag)
- [Ronald Cornet (AmsterdamUMC)](https://github.com/ronaldcornet)
- [Nirupama Benis (AmsterdamUMC)](https://github.com/nirupamabenis)

## Task 13.3
Availability: public
- [Nirupama Benis (AmsterdamUMC)](https://github.com/nirupamabenis)

## Task 14.1
Availability: public
- [Nirupama Benis (AmsterdamUMC)](https://github.com/nirupamabenis)
- [Andra Waagmeester (AmsterdamUMC)](https://github.com/andrawaag)

## Task 16.5
Availability: public
- [Andra Waagmeester (AmsterdamUMC)](https://github.com/andrawaag)
- [Mark Hanauer (Orphanet)](https://github.com/orgs/ERDERA/people/Orphanet)

# Public GitHub repositories
## Work package 16
- [Andra Waagmeester (AmsterdamUMC)](https://github.com/andrawaag)

## Semantic artefacts
- [Andra Waagmeester (AmsterdamUMC)](https://github.com/andrawaag)
### Description
SPARQL examples is intended to be a collection of SPARQL examples for various ERDERA projects. This repository is a fork of the [SIB-Swiss sparql-examples repository](https://github.com/sib-swiss/sparql-examples) and follows the same structure and guidelines. The repository is used to store SPARQL queries in a structured way, with each query stored in a separate file. The queries are stored in the examples folder, with each project having its own subfolder. The repository also contains a README file with information about the project and how to contribute to it.