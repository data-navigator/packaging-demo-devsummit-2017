<section data-background="img/bg_title.jpg">
<h1>Python Package Management in ArcGIS Pro Using Conda</h1>
<br>
<h2>Clinton Dow</h2>
</section>

Overview of Conda in ArcGIS Pro {data-background="img/bg_right.jpg"}
============================================================

What is Conda? {data-background="img/bg_left.jpg"}
--------------------------------------------------------------------

- Python virtual environment and package manager
    - Multiple instances of python.exe and supporting files
    - Easily add/remove 3rd party code to projects
    - Automates dependency handling
- Subset of Anaconda functionality
    - Does not include all packages
    - Command Line Interface only, no GUI
    - Additional features supporting [https://anaconda.org/](https://anaconda.org/ ) 
- Open Source, written in Python
    - [https://github.com/conda/conda](https://github.com/conda/conda)
    - Created by Continuum Analytics
    
![](img/ca.png)


Product Story {data-background="img/bg_left.jpg"}
---------------------------------------------------------

- ArcGIS heavily dependent on Python, shipped with specific version
    - Locked-in to package versions ie: NumPy, SciPy
    - Broken Python env breaks the application
    - No package management
- Python Ecosystem becoming more robust
    - Data Science/Visualization
    - Machine Learning
    - Scientific Libraries
- Desire for enhanced sharing experience
    - Handles requirements
    - Ease of distribution


Terminology {data-background="img/bg_right.jpg"}
============================================================

Virtual Environments {data-background="img/bg_left.jpg"}
------------------------------------------------------------------------------------------------------

- Concept
    - ‘Virtual Machine Lite’
    - Allows multiple side-by-side Pythons on one machine
    - Different configurations for each Python installation
- Conda Environments
    - Package Dependency SAT Solver
        - Satisfiability Solver
    - Stored in the \bin\Python\envs folder within the Pro installation
- Simply a folder on disk, nothing fancy
    - Cheap to create, disposable/iterable
    - Easy to replicate with metadata
    
![](img/envs.jpg)


Packages {data-background="img/bg_left.jpg"}
------------------------------------------------------------------------

- Concept
    - Small units of functionality added to a kernel
    - Unix/Linux concept (apt-get, yum, etc)
    - Not Python exclusive (npm, nuget, etc)
- Versioning Friendly
    - Multiple versions available at one time
    - Each version may depend on different, additional packages
- Similar to shipping a package from a retailer
    - Ingredients, Warning Labels, Instruction Manual
    
![](img/pkg.png)    


Package Structure {data-background="img/bg_left.jpg"}
------------------------------------------------------------------------

![](img/structure.png)

- Python Packaging Authority
    - https://www.pypa.io/en/latest/
    - https://packaging.python.org/distributing/
- Sample Github Project
    - https://github.com/pypa/sampleproject


Channels {data-background="img/bg_left.jpg"}
---------------------------------------------------------------

- Concept
    - A source of related packages
        - A TV channel is a source of related shows
- Public Channel
    - Hosted on anaconda.org
    - Free to create
    - Similar to a public github repository
- Private Channel
    - A webserver which hosts packages
    - As customizable as any other web service
        - Access Control
        - Telemetry

![](img/channels.jpg)


Anaconda.org Contributors and Organizations {data-background="img/bg_left.jpg"}
---------------------------------------------------------------

![](img/anacondaorg.png)

- Similar structure to github organization/user repos


Channels (.condarc file) Structure {data-background="img/bg_left.jpg"}
-------------------------------------------------------------

- Anaconda.org usernames as channel names
- Private Server as http://channel-name
- Local File as file:///file-name

![](img/condarc.png)

Private Repository {data-background="img/bg_left.jpg"}
-------------------------------------------------------------

![](img/repo.png)

- Simply a webserver hosting .tar.bz2 files
- Indexed with ‘conda index’ to create repodata.json


Scalability {data-background="img/bg_left.jpg"}
----------------------------------------------------------------

- Packages easily deploy as webservices
    - Container ecosystem (Docker etc)
- Automate setup of new workstations
    - Saves times for Sys Admins
- Distribute to as few or as many users as required
- Leverage open-source Python packages to save time and costs
    - Thousands of useful packages freely available
- Becoming an industry-standard Python utility
    - Increased familiarity
    - Lowered complexity of onboarding


Looking Ahead {data-background="img/bg_right.jpg"}
================================================================================

ArcGIS Pro 2.0 {data-background="img/bg_left.jpg"}
----------------------------------------------------------------------------

- Enhanced Environment Control in the User Interface
- Integration with R tools and the r-python bridge for ArcGIS


ArcGIS Pro 2.1 {data-background="img/bg_left.jpg"}
--------------------------------------------------------------------

- Adding packaging and channel support
- ArcPy package


Thank you!! Questions/Comments?? cdow@esri.com {data-background="img/bg_title.jpg"}
==============================================================================================