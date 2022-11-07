# Softwaretechnik WS22
 # Java CSV Parser
## Requirements 
Die folgenden Programme/Software müssen*installiert sein
+ Java SDK, Version >11 
	+ aber nicht version 10, da gibt es einen Bug 
+ Maven Version >= 3.x
+ Prettyprint, ~~Version < 2~~
### Installation
Gehe ins root-Verzeichnis und führe folgende Befehle aus
```
<div>mvn install 
```
> _Hinweis: Evtl. muss der absolute Pfad zu maven angegeben werden, falls `mvn` nicht im `PATH` zu finden ist_

&nbsp;

**[...]**

### Usage
```java
import CsvParser.*;  
   
public class Main() {  
   
  public static void main([] args) {  
   
    var parser = new CsvParser();  
    var csvTable = parser.parse(args[0]);  
    System.out.printLn(csvTable);  
  }  
   
}
```
Weitere Beispiele sind bei [github](https://github.com/ "github") zu finden...
 
### Performance

| Programs       | Rows | Runtime   |
|:---|:---|---:|
| Java CSVParser | 1000 | **0.01s** |
|JParse|1000|0.05s|
|Java CSV Parser|1 000 000|**10s**|
|Japrse|1 000 000|50s|

### TODOS
- [x] Readme erstellen
- [ ] Schnittstellen verbessern 
   - [x] allgemein
   - [ ] vom Parser