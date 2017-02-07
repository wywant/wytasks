
#Actions
* reader.string.*
* reader.bytes.*
* servelet.contentType
* servlet.output
* servlet.writer
* servlet.error
* template.engine.velocity
* expression.calculator
* expression.boolean
* string.format
* index.*

##readers
* file : path, encode
* resource : path, ecode
* mysql.table: tableName, keyColumnName, valueColumnName, key
* SnippetPart : key
* JsPart: key
* SnippetJsPart : key
* KeyValueIndexReader : InputStreamFactory, indexName, key

##expression.boolean
* fileExists
* notNull
* greatThan
* lessThan

