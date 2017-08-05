'Umbrella' project that collects various example CRUD applications that share a common HTTP interface.

This project used to host git submodules to individual client and server projects.  Now it just a status information and a lists my interchangeable CRUD projects and has status

__Goals__:  
My goal is to implement the same CRUD using different choices of front-end and back-end technologies.  I want to focus on FP technologies that offer strong static type checking.

_Polymorphism_:   
Is also my big goal. CRUD logic is implemented once and can be used across CRUD entities.  

_Client side hash routing_:  


__Current implementations__:
* [crud-ex-frontend-elm](https://github.com/rpeszek/crud-ex-frontend-elm.git): Elm front-end.
* [crud-ex-frontend-purescript](https://github.com/rpeszek/crud-ex-frontend-purescript) Purescript front end - early stage, current work
* [crud-ex-backend-yesod](https://github.com/rpeszek/crud-ex-backend-yesod.git): Haskell Yesod web app.
* [crud-ex-backend-servant](https://github.com/rpeszek/crud-ex-backend-servant.git): Haskell Servant Web API, back-end and more.
* [crud-ex-backent-http4s](https://github.com/rpeszek/crud-ex-backent-http4s): Scala http4s backend with STM and doobie SQL persistence.

Refer to READMEs in these 'child' projects for more info and to see how to compile/run them.

__TODO List:__  
* Implement security and entity ownership
* Add has-many relationship to example CRUD
* Stricter restful implementation
