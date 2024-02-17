# std::basic_istream<CharT, Traits>

## [operator>>](https://en.cppreference.com/w/cpp/io/basic_istream/operator_gtgt)

* 앞의 whitespaces 는 제거함
* 파라메터가 `short&` 또는 `int&`이고, 입력이 범위 밖이라면, 파라메터는 `std::numeric_limits<T>::max()`또는 `std::numeric_limits<int>::min()`으로 저장되고,  `failbit` 이 설정된다.(unsigned의 경우 두 상황 다 `std::numeric_limits::max()`) .
* 데이터 추출이 실패했을 경우(integer를 받을 때 문자가 입력된 경우 등등) `0`이 저장되며,`failbit` 이 설정된다.