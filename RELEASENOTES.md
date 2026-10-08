## 0.21.0



* added MulleObjCXMLParser, a SAX-style incremental XML parser for feeds, HTML and arbitrary XML
* documented the optional MulleObjCXMLParserDelegate protocol callbacks for elements, character data and parse errors
* documented MulleObjCExpatParser conformance to MulleObjCXMLParserDelegate and its `_error` ivar
* clarified that the property list parser reports XML events through the shared delegate interface


feature: add generic XML parser and fix real number plist output

* new MulleObjCXMLParser class with MulleObjCXMLParserDelegate protocol for SAX-style XML parsing
* supports whole-document parsing via -parseData: as well as incremental/chunked parsing via -parseBytes:length:isFinal:
* add -abortParsing and delegate error reporting through -parser:parseErrorOccurred:
* property list XML printing now emits `<real>` for float values as well, not just double/long double


### 0.20.11



* centralize dependency imports via generic/import.h and include.h
* add MulleObjCExpatFoundation-standalone.m linkable stub
* reorganize API documentation index under asset/dox/api/toc

### 0.20.10

Various small improvements
