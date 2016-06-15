##Persistance best practices
### Speaker: Markus Junginger 

-What do you do with Persistance?

  ###SQLite
  
  + Users: 40%
#####Positive:
  + Toolchain, DB browser
  + No dependecies
  + Self made schema, under
  + more control, SQL queries 
  + debugable data(base)
  + CP Loaders
######Negative:
  - biolerplate code
  - reinventing the wheel(tools do the work alredy)
  - need to write layer for CP
  - no compile time checks
  - manual schema updates
  - maintanance 
  - SQL is another language
  - SQL can get so long
  - testality
  
  ##ORMs
  + Objects Related Mapper
  + Users: 10%
  
  + Examples: greenDAO, DBflow, ORMlite

#####Positive:  
  + biolerplate code
  + reinventing the wheel(tools do the work alredy)
  + no compile time checks
  + sql is another language
  + sql can get so long
  
######Negative:
  - another lib you have to learn
  - potentially performance decrease
  
  ##NoSQL
  + Users: about 4%
  
#####Positive: 
  + no orm 
  + rx support
  + docs
  + tools 
  
  
  
  
  
