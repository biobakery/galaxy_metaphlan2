#Installation instructions for MetaPhlAn2 in a Galaxy environment.
These instructions require the Mercurial versioning system, galaxy, and an internet connection.

#For general information about GraphLan pease refer to:
```
https://bitbucket.org/biobakery/metaphlan2
```
#Installation procedure: MetaPhlAn2  under Galaxy

Go to the ```//usr/local/galaxy-dist/tools```  directory
Clone metaphlan2 by entering the following command    

```hg clone https://george_weingart@bitbucket.org/biobakery/metaphlan2```
 
Clone this repository somewhere: It will create a directory named "galaxy_metaphlan2"

Create a directory named "metaphlan2"  under /galaxy-dist/tools/metaphlan2

Copy member metaphlan2.xml from galaxy_metaphlan2 on to /galaxy-dist/tools/metaphlan2
 

Update member tool_conf.xml  in the galaxy directory adding the following: 
```
   <section name="MetaPhlAn2" id="MetaPhlAn2">
     <tool file="metaphlan2/metaphlan2.xml"/>
  </section>

```
 
Recycle galaxy

#Note:
Once the repository will e upladed to the tool shed, the instructions will be updated accordingly
