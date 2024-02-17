# std::basic_istream<CharT, Traits>

## operator>>

* Skip preceding whitespaces  
* When parameter is `short&` or `int&`, if the input is out of range, the parameter is stored with min/max(respectivly) value, and `failbit` is set.(when the parameter is `unsigned integer`, max is stored) .
* When extraction fails(e.g. a letter was entered where a digit is expected, zero is written to parameter and `failbit` is set.