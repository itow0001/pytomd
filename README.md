###Package Create/Install###
    python setup.py sdist
    cd ../dist
    pip install pytomd-1.0.1.tar.gz
 
****************************
###CLI Info ###
```
    optional arguments:
      -h, --help  show this help message and exit
      -o OUTPUT   location to put README.md
      -p PATH     base path to scan files
      -e          execute the values
      --version   show program's version number and exit
    
    example:
        pytomd -o ./README.md -p ./src -e
```

### How to document code ###
* the first line is an explanation
* all tags within :<anything>: will in become a parameter
* example tags must go at the end and the code most me contained in 3 back-ticks.

```
def Waldo(var):
''' Here is an example of a class <<< explanation
:param var: This is a parameter   <<< tag
:example:                         <<< example tag
\```                              <<< example block --note do not include the escape \
Some example goes here
\```                              <<< example block --note: do not include the escape \
'''
```







**********************************************
 File @ ***/main.py***

None

**********************************************
 File @ ***/pytomd/__init__.py***

Modules __init__.py

**********************************************
 File @ ***/pytomd/__main__.py***

Main entry for pytomd


***def menu***: 

The Menu is here
**********************************************

***def main***: 

This is used in the cli and from a couple places
**********************************************
**********************************************
 File @ ***/pytomd/modules/data.py***

Created on Jul 28, 2016

@author: iitow


***class File***: 

Represents a python file
**********************************************

***class Data***: 

Represents classes, defs of a python file
**********************************************

***def __init__***: 

Constructor
**********************************************

***def add_data***: 

None
**********************************************

***def __init__***: 

Constructor
**********************************************

***def get_tags***: 

None
**********************************************

***def _get_tags***: 

Bolds params and attribs

**:param line:** String

**:param:** regex: raw String
**********************************************

***def _get_example***: 

Bolds params and attribs

**:param line:** String

**:param:** regex: raw String
**********************************************
**********************************************
 File @ ***/pytomd/modules/__init__.py***

None

**********************************************
 File @ ***/pytomd/modules/scanner.py***

Created on May 2, 2016


**:author:** iitow


***class Scanner***: 

scans all python files for attributes
    
**********************************************

***def __init__***: 

Scanner Constructor

**:param base_path:** String, base of git repo

**:param file:** String, to be parsed

**:param output:** String, place to put README.md
**********************************************

***def get_ast***: 

Get ast obj tree
        
**********************************************

***def _scan***: 

Performs the scan & adds markdown
        
**********************************************

***def bold***: 

Bolds params and attribs

**:param line:** String

**:param:** regex: raw String
**********************************************
**********************************************
 File @ ***/pytomd/modules/manager.py***

Created on Jul 28, 2016

@author: iitow


***class Manager***: 

This class manages all files and scanners
    
**********************************************

***def __init__***: 

Manager Constructor

**:param path:** String

**:param output:** String
**********************************************

***def preface_reader***: 

Adds preface to output file
        
**********************************************

***def writer***: 

Performs all writes

**:param lines:** List

**:param type:** String, w,a
**********************************************

***def _files***: 

performs scan on all files

**:param path:** String
**********************************************

***def parse_dataObj***: 

None
**********************************************

***def run***: 

None
**********************************************
**********************************************
 File @ ***/pytomd/modules/transform.py***

Created on Jul 28, 2016

@author: iitow


***def divider***: 

Represents a markdown divider
**********************************************

***def header***: 

Represents a header
**********************************************

***def bold***: 

Bolds 
    
**********************************************

***def inline***: 

Bolds 
    
**********************************************

***def bold_regex***: 

Bolds params and attribs

**:param line:** String

**:param:** regex: raw String
**********************************************