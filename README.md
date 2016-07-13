ReadStat.jl: Read files from Stata, SPSS, and SAS
--

The ReadStat.jl Julia module uses the
[ReadStat](https://github.com/WizardMac/ReadStat) C library to parse binary and
transport files from Stata, SPSS and SAS. All functions return a
[DataFrame](https://github.com/JuliaStats/DataFrames.jl).

To use the module, you first need to ensure that libreadstat.dylib is in
Julia's load path. You can compile it from [ReadStat](https://github.com/WizardMac/ReadStat)

Usage:

```julia
using ReadStat

read_dta("/path/to/something.dta")

read_por("/path/to/something.por")

read_sav("/path/to/something.sav")

read_sas7bdat("/path/to/something.sas7bdat")
```
