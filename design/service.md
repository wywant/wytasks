
#Actions
* reader.string.*
* reader.bytes.*
* servelet.contentType : contentType
* servlet.output : key
* servlet.writer : key
* servlet.error
* template.engine.velocity
* expression.calculator
* expression.calculator.math
* expression.boolean
* string.format : format, parameters
* index.*
* htmlEncode
* parameterSplit
* bytes.convert.widths : fixWidths, differentWidthAmount, types
* bytes.convert.dataReader: types
* convert.toInt
* converts.*

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
* true
* false


