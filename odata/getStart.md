#Wikipedia
https://en.wikipedia.org/wiki/Open_Data_Protocol
##Restful API
Restful API是基于资源而非操作的API

## Resource identification
OData 通过一个叫做Resource identification的url http://host/service 来定位资源。
##The service document
访问Resource identification后返回The service document。
其中包括了entity sets, functions, and singletons， 但我不知道返回functions的目的。
##The metadata document
返回数据通过The metadata document来描述。 The metadata document的url是http://host/service/$metada

##Dynamic resources 
不是很明白
##Resource operation
* GET: Get the resource (a collection of entities, a single entity, a structural property, a navigation property, a stream, etc.).
* POST: Create a new resource.
* PUT: Update an existing resource by replacing it with a complete instance.
* PATCH: Update an existing resource by replacing part of its properties with a partial instance.
* DELETE: Remove the resource.

##Resource representation
支持Json, Atom, XML等
