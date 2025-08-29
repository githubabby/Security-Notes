Injection 

vulnerabilities where an attacker sends untrusted, hostile data to an application's interpreter, changing the meaning of the comands or code and tricking into executing unintended actions.

when?
-user supplied data is not validated,filtered or sanitized by application.
-dynamic queries or non-parameterised calls without context aware escaping are used directly in the interpreter.
-hostile data is used within ORM search parameter to extract additional, sensitive records.
ORM = Object Relational Mapper (like Hibernate, SQLAlchemy, Entity Framework).
-same concept for SQL procedure, if string is used. 

Notes
-dynamic query vs parameterised query
-context aware escaping

Prevention
-the preferred option is to use a safe API, which avoids using the interpreter entirely, provides a parameterised interface.
-Do not use concatenation and exec/execute immediate in stored procedures.
-use positive server-side validation. account number should be a number, use regex. simple validations. not complete defense but can be a layer of security.
-use prepared queries, for any residual dynamic query escape special characters using specific escape syntax for that interpreter.
note: Still can't escape everything. 