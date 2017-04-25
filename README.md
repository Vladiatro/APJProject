# APJProject
Perl parser with metrics.
Usage:
```
java -jar PerlStats.jar directory [csv file]
```
Example:
```
java -jar PerlStats.jar sources info.csv
java -jar PerlStats.jar sources
```
Both will create _info.csv_ (default) file containing metrics from files in the _sources_ directory. The metrics are the following:

* Lines of code
* Scalars
* Arrays
* Hashes
* Branches (non-cyclic)
* Cycles
* String operators (. lt gt ne etc)
* Numeric operators (+ < > != etc)
* Array gets
* Hash gets
* Regexes
* Functions
* Cyclomatic complexity

Not all sources are guaranteed to be processed properly because perl syntax can be modified using extensions.
