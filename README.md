
I hope to keep adding to this project over time (years?) adding replaceable 
front-end and back-end alternatives.

The idea is implement CRUD using a Web API and a comprehensive entity (called a Thing).
That Web API should define both back-end HTTP CRUD interface as well as front-end  
hash URL fragments dispatch. This should allow for replaceable back-end and front-end implementations
working interchangeably with each other.

Currently I have only Elm front-end and Yesod back-end.
Over next few moths my goal is to refine what Thing is and what the CRUD can actually do using just 
these two technologies.

Refer to READMEs in these 'child' projects to see how to compile/run them.

__Note:__  
Submodule projects references here are __likely to be old versions__. To clone use
```
git clone --recursive https://github.com/rpeszek/typesafe-web-polyglot.git
```
and to get the latest version use
```
git submodule update --remote
```
or __navigate to the latest version__ if browsing them on github.  

It appears that setting SHA head ids for subprojects does not work well :-1: with current version of git.
 
