# Data Model
This a website to [SARGON Ontology](https://sargon-n5geh.netlify.app/)

It is composed of the following main entity types categories according to semantical Data model presented in N5GEH project:
- [Device](https://github.com/N5GEH/SARGON/tree/master/Readme/Device). A Device is a physical object to accomplish a particular task. It captures the static attributes which are common in DeviceModel.
- [DeviceModel](https://github.com/N5GEH/SARGON/tree/master/Readme/DeviceModel). It captures the specific Device attributes and categories into main subgroup of [BuildingRealted](https://github.com/N5GEH/SARGON/tree/master/Readme/DeviceModel/BuildingRelated) and [GridRealted](https://github.com/N5GEH/SARGON/tree/master/Readme/DeviceModel/GridRealted).
- [Building](https://github.com/N5GEH/SARGON/tree/master/Readme/Building) coming soon 

## Content
-   [The use of ontology applied to the Energy Domain](#The-use-of-ontology-applied-to-the-energy-domain)
-   [From ontology to CIM(common information Model)](#From-ontology-to-CIM)
-   [SAREF: description and benefit from its usage](#SAREF:-description-and-benefit-from-its-usage)
    - [SAREF in energy domain](#SAREF-in_energy_domain)
     - [Considerations on the necessary SAREF extention](#Considerations-on-the-necessary-SAREF-extention)
- [Data Model](#data-model)
## The use of ontology applied to the Energy Domain
An Ontology represents the description of knowledge from an interest field. The main purpose of ontologies is to represent the objects semantics from a given domain. This objective is achieved by assigning the objects to classes and by describing those, using properties. According to the model of the used ontology, such descriptions are managed by different restrictions. To enable such a description, it is necessary to formally specify components such as individuals (instances of objects), classes, attributes and relations as well as restrictions, rules and axioms. As a result, ontologies do not only introduce a sharable and reusable knowledge representation but can also add new knowledge about the domain.
Some of the major characteristics of ontologies are that they ensure a common understanding of information and that they make explicit domain assumptions. As a result, the interconnectedness and interoperability of the model make it invaluable for addressing the challenges of accessing and querying data in large organizations. Also, by improving metadata and provenance and thus allowing organizations to make better sense of their data, ontologies enhance data quality.

## From ontology to CIM

One of the main features of ontologies is that, by having the essential relationships between concepts built into them, they enable automated reasoning about data. Such reasoning is easy to implement in semantic graph databases that use ontologies as their semantic schemata. 
What’s more, ontologies function like a “brain”. They work and reason with concepts and relationships in ways that are close to the way humans perceive interlinked concepts.
Ontologies allows to capture data in a way that makes their relationships become visible, thanks to the use of Unified Modeling Language (UML). The (UML)  is a general purpose, developmental, modeling language in the field of software engineering that is intended to provide a standard way to visualize the design of a system. UML does not offer a lot of tools to express relationships between objects. Everything that is not an aggregation or generalization is swallowed by the very general term "association". Here's where ontologies use semantics. Semantics is about relationships between signifiers (e.g. words).
Data models are usually defined by UML diagrams. For example, the electrical Common Information Model (CIM)  is defined and maintained as a UML model. It defines a common vocabulary and basic ontology for aspects of the electric power industry. 
The CIM models the network itself using the so called “wires model”, which describes the basic components used to transport electricity. Measurements of power are modeled by another class. These measurements support the management of power-flow at the transmission level and by extension, the modeling of power through a revenue meter on the distribution network. 
The CIM is also used to define messages for the wholesale energy market with the framework for energy market communications, IEC 62325. The European style market profile is a profile derivation from the CIM to harmonize the energy market data exchanges in Europe . 
Ontologies can be described in Ontology Web Language (OWL), a language used for knowledge representation (KR) in a semantic perspective. OWL is a set of markup languages which are designed for use by applications which need to process the content of information, instead of just presenting information to humans. 
The OWL ontology describes the hierarchical organization of ideas in a domain, in a way that can be parsed and understood by software. OWL has more facilities for expressing meaning and semantics than XML, RDF, and RDF-S, and thus OWL goes beyond these languages in its ability to represent machine interpretable content on the Web.
In OWL, it is possible to define new relationships between things. The example below defines a property "madeFromGrapes" which points from a class "wine" to a class "wine grapes". Of course, this "madeFromGrapes" is a much better description of the relationship between a wine and a type of grapes than a simple association.
In a UML diagram the relationship between a man and a dog and a wine and a grape look all the same. OWL, on the other end, allows to define these relationships more specifically, which is important if information should be processed by a computer, as the more information a computer can use for its processing, the better. With data models expressed in UML the depth of information can be very limited. in this respect.
## SAREF: description and benefit from its usage
In the future, domestic and industrial appliances will be intelligent, networked smart devices, forming complete energy consuming, producing and managing systems, based on the integration of products from different vendors and vertical industrial sectors. 
The need for all these connected appliances to be able to communicate among themselves and with the service platforms needs to be addressed. This requires open interfaces. Interoperability is thus a key factor in creating an IoT ecosystem, and the availability of a standardized solution, along with related test suites, will be the essential enabler of the IoT. 
To ensure such systems are technically and commercially successful – and widely adopted – it must be possible to combine appliances from different vendors. These systems will also need to be able to communicate with service platforms from different energy service providers in order to manage and control energy usage.
There have been several efforts in terms of ICT standardization in smart home, energy and IOT like CEN, CENELEC, ETSI, IEC, etc. But most of this standardizations effort focus on a specific aspect of smart system for example CENELEC (European Committee for Electrotechnical Standardization)  perform standardization work to enable domestic appliances improve functionality through the use of network communication like smart grids, smart homes and smart networks.  CEN (European Committee for Standardization)  defines a standard in the IoT environments that focuses on the interfaces between edge data capture technologies and the IoT. However, ETSI (European Telecommunications Standards Institute)  gives us a global standard for ICT and with the support commission, ETSI developed SAREF. 
The “Smart Appliances REFerence” (SAREF)  ontology is a shared model of consensus that facilitates the matching of existing assets (standards/protocols/data models/etc.) in the smart appliances' domain. The SAREF ontology provides building blocks that allows separation and recombination of the different part of ontology depending on specific needs. 
The starting point of SAREF is the concept of Device (e.g., a switch). Devices are tangible objects designed to accomplish one or more functions in households, common public buildings or offices. 
The project covers the following appliances:
•	Home and buildings sensors (temperature, humidity, energy-plugs, energy clams, energy meters, water-flow, water quality, presence, occupancy, air monitors, environmental sensors, CO2 sensors, weather stations, etc.) and actuators (windows, doors, stores). Sensors belonging to appliances are treated individually.
•	White goods, as classified by CECED
•	Rinsing and Cleaning
•	Cooking and Baking
•	Refrigerating and Freezing
•	Vacuum Cleaning
•	Washing and Drying
•	HVAC; heating, ventilation, and air conditioning, plumbing, security and electrical systems, as classified by Eu.bac
•	Lighting, with use cases as defined by LightingEurope (f.k.a. ELC)
•	Micro renewable home solutions (solar panels, solar heaters, wind, etc.
The SAREF ontology offers a list of basic functions that can be eventually combined in order to have more complex functions in a single device. It is the core semantic model for smart appliances, which contains the data elements that are used in more than one domain. 
Since smart appliances can be used in and come from several domains, it is possible that specific data elements for a certain domain are not defined in SAREF. To be able to handle these additional data elements and provide a specific domain with a semantic model that fits all the needs of that domain, there is the possibility to create extensions to SAREF.
The modular conception of the ontology allows the definition of any new device based on building blocks describing functions that devices perform. Furthermore, SAREF can be specialized to refine the general semantics captured in the ontology and create new concepts. The only requirement is that any extension or specialization may comply with SAREF.

### SAREF in energy domain
Concerning Smart Appliances SAREF extension investigation in the energy domain, direct inputs from EEBus  and Energy@home  have been included in SmartM2M developments where Energy, Environment and Building sectors are now part of normative work. SAREF4ENER  is meant to enable the (currently missing) interoperability among various proprietary solutions developed by different consortia in the smart home domain. By using SAREF4ENER, smart appliances from manufacturers that support the EEBus or E@H data models will easily communicate with each other using any energy management system at home or in the cloud. 
Towards this aim, SAREF4ENER should be used to annotate (or generate) a neutral (protocol-independent) set of messages to be directly adopted by the various manufacturers or mapped to their domain specific protocols of choice. SAREF4ENER focuses on demand response scenarios, in which customers can offer flexibility to the Smart Grid to manage their smart home devices by means of a Customer Energy Manager (CEM). 
The CEM is a logical function for optimizing energy consumption and/or production that can reside either in the home gateway or in the cloud. Moreover, the Smart Grid can influence the quantity or patterns of use of the energy consumed by customers when energy-supply systems are constrained, e.g. during peak hours. These scenarios involve the following use cases:
•	Configuration of devices that want to connect to each other in the home network, for example, to register a new dishwasher to the list of devices managed by the CEM.
•	Smart energy management/ (re-)scheduling appliances in certain modes and preferred times using power profiles to optimize energy efficiency and accommodate the customer's preferences
•	Monitoring and Control of the start and status of the appliances;
•	Reaction to special requests from the Smart Grid, for example, incentives to consume more or less depending on current energy availability, or emergencies that require temporary reduction of the power consumption.
These use cases are associated with the user stories according to the IEC TR 62746-2:2015, it describes systems interface between the customer energy management system and the power management system. 
Therefore, there is common agreement between Industry and Research that there is a concrete possibility to proceed with the extension of the SAREF ontology to the subset of this standard related to devices and appliances.

### Considerations on the necessary SAREF extention

The energy sector is experiencing a continuous transformation: data-driven services and functionalities depend more and more on smart devices, which communicate between each other an increasing amount of data. This digitalization process is expanding to domains never considered in this transformation, for which a suitable representation of the system according to the presented SAREF ontology constitutes a valuable advance.
A certain number of domains have been identified as possible targets for extending SAREF. In particular, with reference to the activities conducted in the research projects FISMEP and “National 5G Energy Hub” , the goal of creating SAREF extension in smart energy is to consider the distribution electrical grids and building energy automation domains. 
The initial SAREF extension in smart energy is based on a limited set of use cases and existing data models identified within available initiatives that are summarized below:

   •	Automation of medium voltage distribution grids is considered in the proposed activity, in particular considering the inclusion of Direct Current (DC) technology for which the grid is operated as hybrid AC-DC electrical network. Currently, the standard IEC-61850 constitutes a well-received reference for the automation of distribution grids. The proposed extension consists in reformulating the data structure used in IEC-61850 according to an ontology description, as well as introducing devices specifically related to hybrid AC/DC grids, as power converters or DC switches.
  •    Phasor Measurement Units (PMUs) find more and more application in the monitoring and control of the electrical grid, not only in the transmission networks but also in the distribution ones. The PMUs interaction with the connected devices, as well as the data-driven applications that exploits the obtained measurements, constitute a worthwhile field for the SAREF expansion.
    
   •	The control of energy provision in buildings (as gas, electricity, hot water, etc.) and its optimization involves the deployment of building energy management (BEM) systems, which rely on the interaction with smart meters and actuator devices for the effective operation of each functionality. Moreover, the user involvement in the overall process is an undeniable constituent, which has to be included in the ontology representation of this domain.
   
   •	In order to optimize the overall energy management, the utilities have to expand the energy control to the entire city district, as building agglomeration. New strategies are being developed, considering also the increasing deployment of Distributed Energy Resources (DERs) and the new role of prosumers in the energy market.
   
   •	The proposed SAREF expansion targets also the interaction between the energy management of building/districts and the electrical automation, considering the control functionalities and the data/measurements that involve the combination of both these aspects.


## Data Model
SAREF contains core concepts that are common to several IoT domains and, to be able to handle specific data elements for a certain domain, dedicated extensions of SAREF can be created. Each domain can have one or more extensions, depending on the complexity of the domain. This initial SAREF extension for smart energy will be based on a limited set of use cases and existing data models identified within available initiatives.  The work established with the goal of creating SAREF extensions for the building and grid automation domains. Within the concept of the project, the set of the requirements for an initial semantic model investigated. To do, we

•	Gather requirements, collect use cases and identify existing sources (e.g. standards, data models, ontologies, etc.) from the domains of interest in order to determine the requirements for an initial semantic model for each domain, based on at least 2 use cases and existing data models 
•	Specify and produce the extension of SAREF for each of the aforementioned domain based on the requirements 
In fact, the success of smart grid and smart building/industrial are very much related to interoperability, which means that all smart devices in a home/building/industrial environment have a common understanding of messages and data in a defined interoperability area. In a broader perspective, it does not matter if it is as an energy related message, management message or an informative message.

New applications in Smart Energy domain collates and interprets data from fast-changing and geographically dispersed sources. It also actuates devices and effects many real-world results. To produce, interpret and exchange data, these applications need to define unambiguously the data used, and to share those definitions with other applications. The data relevant to a service, and the definitions that describe its format and meaning, can be called the context of the service. For example, property of devices and application specific information must have common definitions and be understood by all the applications which manipulate it. 

The ETSI Industry Specification Group presents NGSI-LD for cross-cutting Context Information Management [CIM] (https://www.etsi.org/deliver/etsi_gs/CIM/001_099/009/01.01.01_60/gs_CIM009v010101p.pdf) that tackles issue of enabling close to real-time access to information coming from many different sources. The project used the main concepts behind a new data exchange protocol called NGSI-LD which aims to make it easier to find and exchange information with open databases, mobile Apps and IoT platforms. Context information exchange using NGSI-LD has major advantages. Firstly, within the NGSI-LD framework, applications can flexibly discover and query relevant information. 
The data discovery is dynamic, and the built-in query patterns support the most common questions that are practical in unbounded federated information systems. Secondly, NGSI-LD helps to precisely communicate the nature of the context information for a given service, such as its period of validity, its geographic constraints, and other semantically important information, by enabling direct inclusion of pointers to the relevant parameters and definitions. 
To ensure interoperability, the NGSI-LD API defines the meaning of the most commonly needed terms and provides the tools to create domain-specific extensions to model any other type of information. 

Thirdly, NGSI-LD provides a scalable solution to connect, publish and federate diverse data sources using a developer-friendly interface for data sharing and usage. More specifically, the data in NGSI-LD are structured like a data graph model and linked with each other. The relationships between entities are easily handled in NGSI-LD in a similar way to graph databases. It also provides the update, query and subscription support needed to allow applications to automatically access data from various data sources. NGSI-LD builds upon previous work, including OMA and FIWARE.  It is intended to complement and work alongside IoT system specifications, while providing a path to integrate data from open linked data and other information sources.  
In NGSI-LD, information not relevant to the application layer of that particular service, for example details of the IoT or network technologies used to connect entities, or to manage IoT devices and gateways, is not explicitly considered. Such aspects are covered elsewhere, for example in oneM2M, where ETSI is a founding member alongside other major international standards bodies. OneM2M has defined a common platform for IoT, which can interoperate with a wide range of networks and systems. 
The NGSI-LD information model makes it easy to create models of real-world entities, relationships and properties; moreover, the information model is expressive enough to connect and federate other existing information models, using JSON-LD. It is also compatible with RDF so that triple stores and application logic found e.g. in SPARQL or DataCube software can be applied. The NGSI-LD Information Model is defined at two levels, consisting of the Core Meta Model, the Cross-domain Ontology, and the open-ended domain-specific models. In this mothed NGSI-LD Core Meta Model, in the center of the figure, represents Entities, their Relationships, and their Properties with values. It contains the core terms needed to uniquely represent the key concepts of the NGSI-LD Information model as well as the terms that define the API-related Data Types. 
These are encoded using JSON-LD, which provides the advantage of being familiar and accessible to developers. For example, an Entity, representing a device or other data source, is encoded using a JSON-LD object. The NGSI-LD Cross Domain models provide commonly used constructs such as time and geographical location. These are generally applicable to many domains so standardizing their representation provides valuable cross-domain interoperability. 
The main features of the NGSI-LD Cross Domain model have been added to distinguish between: (a) the location of an entity; (b) the entities observation space which is the geographic  location  that  is  being  observed by the entity; and (c) the operation space which is the geographic location in which an entity is active. Domain-Specific Ontologies for entities (real world devices, databases, or other information sources) can be created by extending the Cross-Domain Ontologies and the Core Metamodel, with specialized terms drawn from other ontologies. For instance, the SAREF Ontology which is a shared model of consensus that facilitates the matching of existing assets (standards/protocols/data models/etc.) in the smart appliance's domain. It can be mapped to the NGSI-LD Information Model, so that smart home applications will benefit from this Context Information Management API specification. 


With respect to the aforementioned concept, data models have been harmonized to enable data portability for different applications in smart energy system including, but not limited, to building automation and power grid controlling/monitoring. They are intended to be used together with  FIWARE NGSI-LD. The data model is covering Building and Device domains and connecting these two domains according to the concept of Linked-data. Two main classes are related to Device and Building.  Two main classes are related to Device and Building.  A Device is a tangible object, which contains some logic and is producer and/or consumer of data. The device itself categorized into the building related or grid related. Based on this category of devices, a bottom up approach is taken to define an entity within the platform. Each model of device inherent from class Device and has own private properties. Context information of data model exists on https://fiware.n5geh.de/ngsi-ld/ and Figure ? represents the graph visualization of data model with a view of classes in Web Protégé.  

 <img src="Images/protege.png" width=850> 
 
# License

- [MIT-License](LICENSE)

# Copyright

2020, RWTH Aachen University, E.ON Energy Research Center, Institute for Automation of Complex Power Systems

# Contact

[![EONERC EBC_Logo](https://www.ebc.eonerc.rwth-aachen.de/global/show_picture.asp?id=aaaaaaaaaakevlz)](https://www.acs.eonerc.rwth-aachen.de)

- [Maliheh Haghgoo](https://www.acs.eonerc.rwth-aachen.de/cms/E-ON-ERC-ACS/Das-Institut/Mitarbeiter/Energy-Management-Systems-Data-Analyti/~ohbu/Haghoo-Maliheh/lidx/1/)

[Institute for Automation of Complex Power Systems(ACS)](https://www.acs.eonerc.rwth-aachen.de)  
[EON Energy Research Center (EONERC)](http://www.eonerc.rwth-aachen.de)  
[RWTH University Aachen, Germany](http://www.rwth-aachen.de)


# Acknowledgement
<img src="https://www.ebc.eonerc.rwth-aachen.de/global/show_picture.asp?mod=w%3d474%26h%3d%26gray%3d%26neg%3d%26mirror%3d%26flip%3d%26rleft%3d%26rright%3d%26r180%3d%26crop%3d%26id%3daaaaaaaaaayxgwf&id=aaaaaaaaaayxgwf" width="250">

We gratefully acknowledge the financial support provided by the BMWi (Federal Ministry for Economic Affairs and Energy), promotional reference 03ET1561A/B/C





