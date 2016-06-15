We made an interactive session on persistence

Plain SQLite
============
~40% of the audience use it

+ Toolchain, e.g. DB browser
+ No dependencies 
+ Self made schema, under
+ Dev as full control, e.g. SQL queries
+ debuggable data(base)
+ CP and Loaders
- A lot of boilerplate code
- Reinventing the wheel (tools do the work already)
-(+) Need to write layer for CP, however close to CP with Cursors, etc. 
- no compile time checks
- manual schema updates maintenance
- SQL is another lang
- SQL can get loooooong
- Testablilty?

ORMs (Object/Relational Mappers
====
~10% of the audience use it

greenDAO (robust: around since 2011, fastest ORM) 
DbFlow ()
ORMLite 
Requery (quite new, beta, RX support)

Delta to SQLite
---------------
+ less biolerplate code
+ not reinventing the wheel (tools do the work already)
+ compile time checks
+ no to less sql
- another lib you have to learn
- potentially performance decrease (depends on the lib)

Realm
=====
~ 4% of the audience use it
+ No ORM (?, technically it's an ORM to its own native database)
+ RX support
+ Docs
+ Tools

Others
======
~ 1% of the audience use it
