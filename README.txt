JSON Parser in C

4 function

json_parser_parse
json_parser_value
json_parser_pair
json_parser_ignore

usage:

json_parser_parse(root)

if (root.type == JSON_OBJECT) {
	for (;;) {
		json_parser_pair(name, value)
	}
} else if (root.type == JSON_ARRAY) {
	for (;;) {
		json_parser_value(element)
	}
}

if don't need object or array call `json_parser_ignore`

more demo see github.c require libcurl

License:
Public Domain
