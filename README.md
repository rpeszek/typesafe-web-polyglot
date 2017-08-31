'Umbrella' project that collects various example CRUD applications that share a common HTTP interface.

This project used to host git submodules to individual client and server projects.  Now it just a status information and a lists my interchangeable CRUD projects and has status

__Goals__:  
My goal is to implement the same CRUD using different choices of front-end and back-end technologies.  I want to focus on FP technologies that offer strong static type checking.

_Polymorphism_:   
Is also my big goal. Various aspects of CRUD logic are implemented once and can be used across CRUD entities.  CRUD == no business logic so things stay somewhat dull.

_Client side hash routing_:  
CRUD components are agnostic of each other existence, presentation is dispatched using hash URL routing.

__Current implementations__:
* [crud-ex-frontend-elm](https://github.com/rpeszek/crud-ex-frontend-elm.git): Elm front-end.
* [crud-ex-frontend-purescript](https://github.com/rpeszek/crud-ex-frontend-purescript) PureScript front-end.
* [crud-ex-backend-yesod](https://github.com/rpeszek/crud-ex-backend-yesod.git): Haskell Yesod web app.
* [crud-ex-backend-servant (master)](https://github.com/rpeszek/crud-ex-backend-servant.git): Haskell Servant Web API, back-end and more on master branch.
* [crud-ex-backend-servant (eta-jetty)](https://github.com/rpeszek/crud-ex-backend-servant/tree/eta-jetty): [Eta](http://eta-lang.org/) port that runs in jetty server on eta-jetty branch.
* [crud-ex-backent-http4s](https://github.com/rpeszek/crud-ex-backent-http4s): Scala http4s backend with STM and doobie SQL persistence.

Refer to READMEs in these 'child' projects for more info and to see how to compile/run them.

__TODO List:__  
* Implement security and entity ownership
* Add has-many relationship to example CRUD
* Stricter restful implementation
