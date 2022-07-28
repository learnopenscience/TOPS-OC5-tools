# Lesson 3: Open Science tools for reproducibility

```{contents}
:local:
```

## Introduction 

This lesson is the third of the OpenCore Open Science Tools and Resources Modules. In this lesson, we'll take a deep dive into the tools for (computational) reproducibility. 

Ensuring the reproducibility of research tools are an intrinsic and complicated piece of the Open Science puzzle. In order to understand what reproducible research tools are, we first need to define what reproducibility means for different platforms, methods, and data. 

[The Turing Way 'Guide to Reproducible Research'](https://the-turing-way.netlify.app/reproducible-research/reproducible-research.html)

### 3.1 What is reproducibility?

The [National Academies (2019)](https://www.nationalacademies.org/our-work/reproducibility-and-replicability-in-science) define *computational reproducibility and repeatability* as the following:

reproducibility  
:  as obtaining consistent computational results using the same input data, computational steps, methods, code, and conditions of analysis.
  
replicability
: obtaining consistent results across studies aimed at answering the same scientific question, each of which has obtained its own data. 

```{admonition} Plesser (2017) definitions 
:class: dropdown
In [Reproducibility vs. Replicability: A Brief History of a Confused Terminology](https://doi.org/10.3389%2Ffninf.2017.00076), Plesser (2017) gives the following useful definitions:

repeatability
: (Same team, same experimental setup): The measurement can be obtained with stated precision by the same team using the same measurement procedure, the same measuring system, under the same operating conditions, in the same location on multiple trials. For computational experiments, this means that a researcher can reliably repeat her own computation.
            
replicability
: (Different team, same experimental setup): The measurement can be obtained with stated precision by a different team using the same measurement procedure, the same measuring system, under the same operating conditions, in the same or a different location on multiple trials. For computational experiments, this means that an independent group can obtain the same result using the author’s own artifacts.

reproducibility
: (Different team, different experimental setup): The measurement can be obtained with stated precision by a different team, a different measuring system, in a different location on multiple trials. For computational experiments, this means that an independent group can obtain the same result using artifacts which they develop completely independently.

Plesser (2017) goes on to further simplify reproducibility into:

methods reproducibility
: provide sufficient detail about procedures and data so that the same procedures could be exactly repeated.

results reproducibility
: obtain the same results from an independent study with procedures as closely matched to the original study as possible.

inferential reproducibility
: draw the same conclusions from either an independent replication of a study or a reanalysis of the original study.
```

[Peng (2011)](https://doi.org/10.1126/science.1213847) provides us with the following figure on reproducibility as a "*spectrum of practices*".

![peng_2011](../assets/reproducibility-spectrum-peng-2011.png)

In considering computational reproducibility, we must consider more than just providing the public with a well written methods section in a peer-reviewed publication or raw data. Providing the software description - ideally free and open source software, as well as a computational environment in which the work can be re-analyzed become necessary steps. Achieving "reproducible research" greatly benefits from initiating open science best practices at the beginning of a new research project. However, helping existing research projects or long term observatory datasets become more reproducible are all possible *post-hoc*. 

#### Licenses

Licenses for scientific software and scientific data are strongly encouraged. Adding a license to your work encourages the following things to happen (and just as importantly: not to happen): 

Without a defined licenses other individuals or groups can file for copyright or patents on these intellectual property, techniques, or even molecular and genetic material. 

In order for Software, Code, and Research Data remain free and open they require permissive, open source, open science compliant licenses be provided along side them.

```{admonition} License Types
:class: dropdown
[FAQ Creative Commons Licenses](https://wiki.creativecommons.org/wiki/Data#Frequently_asked_questions_about_data_and_CC_licenses)

[Creative Commons Licenses](https://creativecommons.org/licenses/)

[Open Source Initiative Licenses](https://opensource.org/licenses)

[ChooseALicense.com](https://choosealicense.com/)
```

#### Data Reproducibility

In the context of open science, reproducibility of scientific data is dependent upon data which meet or exceed the definitions of FAIR & CARE. 

In order for data to meet the requirements of FAIR & CARE they need to be searchable. Data which have been indexed by search engines and have machine readable metadata increase their likelihood of being FAIR.

[Open Knowledge Foundation's OpenData Handbook](http://opendatahandbook.org/)

##### Protocols and Bench Techniques

The(re)creation of data is critical to the scientific process and to reproducibility. There are many excellent open resources for developing and publishing open source scientific protocols and bench techniques:

```{admonition} List of Protocol websites
:class: dropdown
[BioProtocol](https://bio-protocol.org/Default.aspx)

[Current Protocols](https://currentprotocols.onlinelibrary.wiley.com/)

[Gold Biotechnology Protocol list](https://www.goldbio.com/search?q=&type=documentation&documentation_type=protocol)

[JoVE](https://www.jove.com/) - Journal of Visualized Experiments

[Nature Protocols](https://www.nature.com/nprot/)

[OpenWetWare](https://openwetware.org/wiki/Main_Page)

[Protocol Exchange](https://protocolexchange.researchsquare.com/)

[Protocols Online](http://www.protocol-online.org/prot/)

[Protocols](https://www.protocols.io/)

[SciGene](http://scigine.com/blog/)

[Springer Nature Experiments](https://experiments.springernature.com/)
```

#### Data Findability

In order for data to be findable, they must have metadata which can be "crawled" by internet search engines. These metadata take the form of machine readable content or "schema" which allow for structured search queries. 

Metadata that have an "[ontology](https://en.wikipedia.org/wiki/Ontology_(information_science))" of associated terms and how they relate to one another allow for knowledge graphs to link related terms together.

```{admonition} Search Engines
:class: dropdown
[OpenAire](https://explore.openaire.eu/search/find/dataproviders)

[OSF Share](https://share.osf.io/sources)
```

```{admonition} Structured Search
:class: dropdown
[Schema.org](https://schema.org/)

[Sustainability Data](https://blog.google/outreach-initiatives/sustainability/data-commons-sustainability/)

[DataCommons.org](https://datacommons.org/)

[Linked Open Data Cloud](https://lod-cloud.net/)
```

```{admonition} Scientific Knowledge Graphs
:class: dropdown
[AIDA](http://w3id.org/aida) -  Academia/Industry DynAmics (AIDA) Knowledge Graph, which describes 21M publications and 8M patents according to the research topics drawn from the Computer Science Ontology.

[Open Knowledge Graph](https://data.open.ac.uk/)

[Open Research Knowledge Graph](https://www.orkg.org/orkg/)

[Amazon Science](https://www.amazon.science/tag/knowledge-graphs)
```

```{admonition} Literature & Document Search
:class: dropdown
[Google Scholar](https://scholar.google.com/intl/en/scholar/about.html) - based on Google's powerful knowledge graph

[Bieleld Academic Search Engine (BASE)](https://www.base-search.net/) - provides more than 240 million documents from more than 8,000 content providers.

[BioOne](https://bioone.org/)

[CERN Document Server](https://cds.cern.ch/?ln=en)

[CiteSeerX](http://citeseerx.ist.psu.edu/index)

[CORE](https://core.ac.uk/) - currently contains 207,255,818 open access articles collected from 10,591 data providers around the world.

[DeepDive](http://deepdive.stanford.edu/)
    
- [PaleoDeepDive](http://deepdive.stanford.edu/paleo)
     
- [GeoDeepDive](https://geodeepdive.org/)

[Directory of Open Access Journals](https://doaj.org/) -  a community-curated online directory that indexes and provides access to high quality, open access, peer-reviewed journals.

[Mendeley(Elsevier)](https://www.elsevier.com/solutions/mendeley)

[Microsoft Academic Research](https://www.microsoft.com/en-us/research/project/academic/)

[Organic ePrints](https://orgprints.org/) -  is an international open access archive for papers and projects related to research in organic food and farming. 

[PubMed](https://pubmed.ncbi.nlm.nih.gov/)

[ResearchGate](https://www.researchgate.net/)

[Science.gov](https://www.science.gov/)

[ScienceDirect](https://www.sciencedirect.com/)

[ScienceOpen](https://www.scienceopen.com/)

[Scopus](https://www.scopus.com/home.uri)

[Semantic Scholar](https://www.semanticscholar.org/)

[SSRN](https://www.ssrn.com/index.cfm/en/) - formerly Social Science Research Network, now owned by Elsevier

[UpToDate](https://www.uptodate.com/contents/search)
```

```{admonition} Query Languages
:class: dropdown
[Web Ontology Language (OWL)](https://www.w3.org/OWL/)

[Resource Description Framework (RDF)](https://www.w3.org/RDF/) - the RDF is a World Wide Web Consortium (W3C) standard originally designed as a data model for metadata.

[SPARQL](https://www.w3.org/TR/rdf-sparql-query/)

[GeoSPARQL](https://www.ogc.org/standards/geosparql)
```

##### Publishing Data

There are dozens of scientific projects supporting open science who are hosting their data online


```{admonition} Scientific Data Repositories and curated lists
:class: dropdown
[Open Access Directory](http://oad.simmons.edu/oadwiki/Data_repositories) - curated list of open data repositories

[CyVerse Data Commons](https://cyverse.org/data-commons) - US NSF funded cyberinfrastructure for life sciences

[EDUAT](https://www.eudat.eu/) – network of European research organizations.

[Harvard Dataverse](https://dataverse.harvard.edu/) – offers free storage of research data, owned by Harvard University

[Zenodo](https://zenodo.org/) – EU-funded project by OpenAire, it is hosted by CERN. Useful for EU-funded projects because reports back to the EU research Participant Portal.

[Dryad](https://datadryad.org) – started as US NSF project, used for data sets of any type that correspond to a research paper. 

[Registry of Research Data Repositories](https://www.re3data.org/)

[PLOS Recommended Repositories](https://journals.plos.org/plosgenetics/s/recommended-repositories)
```

```{admonition} Public Data Archives
:class: dropdown
**Agricultural Data**

[Berkeley Library Agricultural and Resource Economics](https://guides.lib.berkeley.edu/ARE/finddata)

[Data.World Data List](https://data.world/datasets/agriculture)

[Farmers.gov](https://www.farmers.gov/data)

[USDA Ag Data Commons](https://data.nal.usda.gov/) - US Department of Agriculture data commons providing central access to USDA's Open Research Data

[USDA Forest Service Data Clearinghouse](https://data.fs.usda.gov/geodata/edw/index.php)

[USDA Forest Service ArcGIS Data](https://data-usfs.hub.arcgis.com/)

[World Bank Ag Data](https://data.worldbank.org/indicator)

**Biological Data**

[European Molecular Biology Laboratory (EMBL)](https://www.ebi.ac.uk/) - European Bioinformatics Institute (EMBL-EBI) 

[Global Biodiversity Information Facility](https://www.gbif.org/)

[National Center for Biotechnology Information](https://www.ncbi.nlm.nih.gov/)

[NIHM](https://www.nimhgenetics.org/)

**Public Data on Commercial Cloud**

[Earth on AWS](https://aws.amazon.com/earth/) - The Registry of Open Data on AWS helps you discover and share datasets that are available via AWS resources. 

[Google Earth Engine](https://earthengine.google.com/noncommercial/)

[Microsoft Planetary Computer](https://planetarycomputer.microsoft.com/)

**US Government Data**

[GeoPlatform.gov](https://www.geoplatform.gov/)

[US Government Public Data](https://data.gov/)

[EPA Data](https://www.epa.gov/data)

[NASA Data](https://data.nasa.gov/)

[USGS data](https://data.usgs.gov/datacatalog/)

**EU Government Data**

[European Space Agency Data](https://earth.esa.int/eogateway)

[Copernicus Climate Data Store](https://cds.climate.copernicus.eu/#!/home)

**Ecological Research Data Repositories**

[eBird](https://science.ebird.org/en/use-ebird-data/download-ebird-data-products) - provides open data access in several formats to logged-in users, ranging from raw data to processed datasets geared toward more rigorous scientific modeling.

[Environmental Data Initiative](https://environmentaldatainitiative.org/) - repository for [Long Term Ecological Research (LTER)](https://lternet.edu/using-lter-data/) network as well as community contributed datasets

[FLUXNET](https://fluxnet.org/)

[Long Term Agricultural Research(LTAR)](https://data.nal.usda.gov/long-term-agroecosystem-research) 

[National Ecological Observatory Network (NEON)](https://data.neonscience.org/) 

[NCAR/UCAR data](https://rda.ucar.edu/) - National Center for Atmospheric Research / National Center for Atmospheric Research data archive.

[US National Phenology Network](https://www.usanpn.org/data)

**Earth Observation System & Weather Data**

[Multi-Mission Algorithm and Analysis Platform (MAAP)](https://www.earthdata.nasa.gov/esds/maap)

[NOAA data](https://data.noaa.gov/datasetsearch/)

- [NOAA Climate data](https://www.ncdc.noaa.gov/cdo-web/)

[UK Met Office data](https://www.metoffice.gov.uk/research/climate/maps-and-data/data/index)

**Open Street Map Data Sets**

[OpenStreetMap (OSM)](https://www.openstreetmap.org/)

[OSM US Forest Service](https://wiki.openstreetmap.org/wiki/US_Forest_Service_Data)

**Web Data Standards**

[W3C](https://www.w3.org/)

[EDM Council](https://edmcouncil.org/)

**Publishing Data Guides**

[FigShare](https://figshare.com/)

[Nature Data Repository Guidance](https://www.nature.com/sdata/policies/repositories)

[Registry of Research Data Repositories (re3data)](https://www.re3data.org/)

[PLOS data](https://plos.org/open-science/open-data/)
```

#### Software Reproducibility

Replication of software environments across hardware types and geographic location (e.g., data centers, universities, research labs) remaines an obstacle to reproducibility, and has for much of the history of research computing. 

Solutions to making software environments more reproducible include the use of virtualization (e.g., virtual machines, containers, virtual environments). 

Software versioning and compiliation of software environments for specific types of hardware architecture (i.e., ARM, X86, GPU, TPU) will continue to evolve over time. 

##### Operating Systems

Operating Systems (OS) are the primary means of interacting with computational hardware and storage for research. Selecting an OS that enables reproducible research is one way of making your science more open.

In 1991, the open source OS [Linux](https://www.linux.org/) was released by Linus Torvalds. Today, Linux is [the most widely used OS for mobile, and importantly for cloud](https://en.wikipedia.org/wiki/Usage_share_of_operating_systems). A significant portion of research software and web development are being written in Linux for distribution over the internet. 

```{admonition} Linux OS
:class: dropdown
[Android](https://www.android.com/)

[Chrome OS](https://www.google.com/chromebook/chrome-os/)

[Debian](https://www.debian.org/)

[Redhat](https://www.redhat.com/en)

[Rocky](https://rockylinux.org/)

[Ubuntu](https://ubuntu.com/)
```

Commercially held, [Apple](https://apple.com) supports its own OS for desktop (Max OS X) and mobile (iOS), which are based on UNIX, and are interoperable with Linux systems.

```{admonition} Apple OS
:class: dropdown
[MacOS X](https://www.apple.com/macos)

[iOS](https://www.apple.com/ios)
```

Commercially held, [Microsoft](https://www.microsoft.com) supports its popular [Windows OS](https://www.microsoft.com/en-us/windows) for desktop computing. Windows is not based on Linux but has built its own [Windows Subsystem for Linux 2 (WSL2)](https://docs.microsoft.com/en-us/windows/wsl/install) which allows for Windows OS users to interface directly with Linux software.

##### Scientific Programming Languages

Writing scientific software takes place within an ecosystem of multiple general purpose, and high-level interpreted programming languages. Just like human society, we all speak and write in a variety of different languages, each with their own strengths and weaknesses. There may never be a single computer language for science, and if there ever was one, surely someone out there would create a new language and proclaim it to be better than the old one.

```{admonition} Common Scientific Programming Languages
:class: dropdown
[UNIX Shell](https://en.wikipedia.org/wiki/Unix_shell) also known as "the command line" or "terminal" is one of the original fundamental interfaces for working with computers remotely. 

- [BASH](https://www.gnu.org/software/bash/) is the GNU Project's shell—the Bourne Again SHell

[C](https://www.iso.org/standard/74528.html) is a general-purpose computer programming language.

[C++](https://isocpp.org/) is a general-purpose programming language.

[C#](https://docs.microsoft.com/en-us/dotnet/csharp/) is a general-purpose, multi-paradigm programming language.

[Fortran](https://fortran-lang.org/) was designed from the ground up for computationally intensive applications in science and engineering. Fortan is one of the most widely used languages for large scale models given its efficient use of memory and its blazing speed. 

- [LFortran](https://lfortran.org/) is a modern open-source (BSD licensed) interactive Fortran compiler built on top of [LLVM](https://llvm.org/). It can execute user’s code interactively to allow exploratory work (much like Python, MATLAB or Julia) as well as compile to binaries with the goal to run user’s code on modern architectures such as multi-core CPUs and GPUs.

[Go](https://go.dev/) is an open source programming language supported by Google.

[HTML](https://html.spec.whatwg.org/) is a markup language used for structuring and presenting content on the World Wide Web.

[JavaScript](https://www.javascript.com/) is the programming language of the Web.

[JSON](https://www.json.org/json-en.html) - JavaScript Object Notation is a lightweight data-interchange format.

- [GeoJSON](https://geojson.org/) JSON extension for geospatial data

[Julia](https://julialang.org/) is a high-level, high-performance, dynamic programming language.

[Make](https://www.freebsd.org/cgi/man.cgi?query=make) is a build automation tool that automatically builds executable programs and libraries from source code by reading files called Makefiles which specify how to derive the target program.

[CMake](https://cmake.org/) is an open-source, cross-platform family of tools designed to build, test and package software. 

[PERL](https://www.perl.org/) is a family of two high-level, general-purpose, interpreted, dynamic programming languages. 

[Python](https://www.python.org/) is a high-level, interpreted, general-purpose programming language. 

[R](https://www.r-project.org/) is a programming language for statistical computing and graphics.

[YAML](https://yaml.org/) "YAML Ain't Markup Language" used in configurations for applications. 
```

##### Documentation Software

Scientific software tools for reproducibility can also include integrated development environments and sharing platforms.

```{admonition} Popular productivity software for documentation
:class: dropdown
[CryptPad](https://cryptpad.fr/) - online rich text pad. 

[Draw.io](https://about.draw.io/) - drawings and diagrams in browser.

[Excel](https://www.microsoft.com/en-us/microsoft-365/excel) - love it or hate it, many people still work in it or with `.xlsx` format files. 

[Google Docs](https://www.google.com/docs/about/) - is an online word processor included as part of the free, web-based Google Docs Editors suite offered by Google.

[HackMD](https://hackmd.io) - online markdown editor.

[JupyterBook](https://jupyterbook.org/en/stable/intro.html) - create documentation using Jupyter Notebooks and Markdown

[MkDocs](https://www.mkdocs.org/) - is a fast, simple and downright gorgeous static site generator that's geared towards building project documentation.

[LaTeX](https://www.latex-project.org/) -  is a high-quality typesetting system

[Overleaf](https://www.overleaf.com/) - LaTeX online document sharing platform.

[ReadTheDocs](https://readthedocs.com/) - documentation using a variety of Markup langages

[Software Heritage](https://www.softwareheritage.org/) - preserves software source code for present and future generations.
```

##### Project Management

```{admonition} Popular productivity software for project management
:class: dropdown
[Atlassian](https://www.atlassian.com/)

- [Confluence](https://www.atlassian.com/software/confluence)

- [Jira](https://www.atlassian.com/software/jira)

- [Trello](https://trello.com/en)

[GitHub Issues](https://github.com/features/issues)

[Open Project](https://www.openproject.org/)

[ZenHub](https://www.zenhub.com/)
```

##### Version Control

Version Control refers to keeping track of the version of a file, set of files, or a whole project.

Examples of version control tools in every day productivity software which you may already use:

* [Microsoft Office Track Changes](https://support.microsoft.com/en-us/office/track-changes-in-word-197ba630-0f5f-4a8e-9a77-3712475e806a)
* [Apple's Time Machine](https://www.apple.com/us/search/Time+Machine)
* [Google Docs Version History](https://support.google.com/a/users/answer/9308971)

Version control is as much a philosophy as it is a set of tools. 

You don't need to master [`git`](https://git-scm.com/) (also [created by Linus Torvalds](https://en.wikipedia.org/wiki/Git)) to utilize version control - although it is certainly a worthwhile tool for many research software engineers and data scientists:

`Git` is the most widely used version control platform for software and code development.

```{admonition} Popular Version Control platforms
:class: dropdown
* [GitHub](https://github.com) -  a distributed version control system based on `git`. GitHub is the most popular platform and the most preferred tool among developers world wide.

* [GitLab](https://github.com) - is an open-core company, provides a DevOps software package that combines the ability to develop, secure, and operate software in a single application. GitLab has [Continuous Integration/Continuous Delivery (CI/CD)](https://docs.gitlab.com/ee/ci/introduction/) and [DevOps workflows](https://about.gitlab.com/topics/devops/) built-in.

* [Source Forge](https://sourceforge.net/) - 

* [Apache SubVersion](https://subversion.apache.org/)
```

### 3.2 Computational Notebooks

A notebook interface (also called a computational notebook) is a virtual environment used for writing descriptive text (conventional writing), code, and data visualization. Notebooks are a form of literate programming which extends to computer consoles and interactive computing. 

```{admonition} Common Notebook types
:class: dropdown
[Apache Spark](https://spark.apache.org/docs/latest/index.html) is a unified analytics engine for large-scale data processing which can use notebook style inputs.

[Apache Zepplin](https://zeppelin.apache.org/) - multipurpose notebooks developed for use with Apache Spark

[iPython](https://ipython.org/) - The original python notebook `.ipynb`

[Jupyter](https://jupyter.org/) - built upon the `.ipynb` the original web application for creating and sharing computational documents. 

[Quarto](https://quarto.org/) - the newer type of Markdown style notebook developed by RStudio, `.qmd`

[R Markdown](https://rmarkdown.rstudio.com/) - `.rmd`
```

#### VS Code

[Microsoft's Visual Studio Code (VS Code)](https://code.visualstudio.com/) is the most popular IDE for software developers in the world. VS Code's tool modularity allows extensions to be developed and added to installations quickly and easily. 

VS Code also supports popular Notebook types (`.ipynb`, `.qmd`, `.Rmd`), Docker, Kubernetes, and remote `ssh` connections which make it one of the most powerful IDE for data scientists working with remote systems and cloud native applications. 

Another benefit of VS Code is that it allows Windows users to connect seamlessly to Linux OS on the cloud.

[GitHub's CodeSpace](https://visualstudio.microsoft.com/services/github-codespaces/) and [GitPod](https://www.gitpod.io/docs/ides-and-editors/vscode) both use VS Code as their default IDE

```{admonition} Popular VS Code Software & Extensions
:class: dropdown

[Jupyter in VS Code](https://code.visualstudio.com/docs/datascience/jupyter-notebooks)

[R in VS Code](https://marketplace.visualstudio.com/items?itemName=REditorSupport.r)

[Quarto in VS Code](https://quarto.org/docs/tools/vscode.html)

[customized notebooks](https://code.visualstudio.com/blogs/2021/11/08/custom-notebooks)

[viatsko/Awesome-VSCode](https://github.com/viatsko/awesome-vscode)

```

#### Jupyter 

[Project Jupyter](https://jupyter.org/) is a community run project with a goal to "develop open-source software, open-standards, and services for interactive computing across dozens of programming languages". It was spun off from IPython in 2014 by Fernando Pérez and Brian Granger.

Today Jupyter is one of the most popular Notebook formats, and has been widely adopted by the Earth Science Community.

Jupyter Notebooks can be loaded in a variety of IDE including the Jupyter Lab, VS Code, and browser based applications.

```{admonition} Popular Jupyter Software & Extensions
:class: dropdown

```

#### RStudio

RStudio created [R Markdown](https://rmarkdown.rstudio.com/) (`.rmd`) a format for writing reproducible, dynamic reports with R.

```{admonition} Popular R Markdown Software & Extensions
:class: dropdown

[R Markdown Lessons](https://rmarkdown.rstudio.com/lesson-1.html)
```

**Quarto**

Recently, [Posit.io](https://posit.co/) released [Quarto](https://quarto.org/) an open-source scientific and technical publishing system built on Pandoc.

#### Cloud Services

There are numerous free and starter-tier cloud services which allow you to run computational notebooks. Most of these offer small virtual machine sizes which are appropriate for viewing notebooks and conducting small

[Google's CoLab](https://colab.research.google.com/)

[MyBinder](https://mybinder.org/)

[GitHub CodeSpaces](https://github.com/features/codespaces/)

[GitPod](https://www.gitpod.io/)

[RStudio Workbench](https://www.rstudio.com/products/workbench/)

## Conclusion

## Assessment

**Scenario 1**: You stumble upon a research paper published a few years ago which used LANDSAT data and techniques similar to a project idea you want to apply for another area of interest. When you read the methods section of the paper, you find they published their derived data set in an international data repository (Dryad), but their algorithm code to generate the processed data from LANDSAT Real-Time (raw) data are not provided, only the description of the technique which they used is given in their Methods section and the mathematical equations for calculating their new index are in the Supplementary Materials.

```{admonition} Question 1
When you can access the raw data, results data, and some written methods: does the research meet the definition of being reproducible?
```{admonition} Answer
:class: dropdown
No, the paper fails to provide a necessary level of detail to allow a different team, with a different experimental setup to obtain the same results exactly. The paper may support some aspects of “Replicability”, but only if someone is able to write their own code using the provided methods. With the same raw data product you could test your code and compare your results data to their results data. This would not be easy and is prohibitive.  
```
```
