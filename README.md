'Umbrella' project that collects various example CRUD applications that share a common HTTP interface.

__Goals__:  
My goal is to implement the same CRUD using different choices of front-end and back-end technologies.  I want to focus on technologies that offer strong static type checking and functional programming benefits.

The glue that holds all of this together is a web API which defines both back-end HTTP interface as well as front-end hash URL-fragment dispatch. 
This web API could be either hand-coded independently in each of the implementations or generated from a common type definition (e.g. Servant API to Elm).

__Current implementations__:
* [crud-ex-frontend-elm](https://github.com/rpeszek/crud-ex-frontend-elm.git): Elm front-end.
* [crud-ex-backend-yesod](https://github.com/rpeszek/crud-ex-backend-yesod.git): Haskell Yesod web app.
* [crud-ex-backend-servant](https://github.com/rpeszek/crud-ex-backend-servant.git): Haskell Servant Web API, back-end and more.

Refer to READMEs in these 'child' projects to see how to compile/run them.

__Git:__  
Each of the implementations has its own project and is listed here as a submodule. To clone use
```
git clone --recursive https://github.com/rpeszek/typesafe-web-polyglot.git
```
and to get the latest version (see nested submodules below) try
```
git submodule update --remote --recursive
```
or __navigate to the latest version__ if browsing them on github.  

*Nested Submodules*  
Because my Elm project uses a package that has not been migrated to Elm v.018, I had to include that dependency as a submodule.  Thus, I have a nested submodule situation and git commands (including git submodule update --init --recursive) do not seem to work well.  Either clone this project again or run an explicit 
```
git clone https://github.com/benthepoet/elm-purecss.git
```
in the crud-ex-frontend-elm/dependencies folder.  I will try to get rid of nested submodules moving forward.
