# Get the Java version

Get the Java version

## Usage

``` r
get_java_version()
```

## Value

the Java version

## Author

Richèl J.C. Bilderbeek

## Examples

``` r

if (is_beast2_installed() && beautier::is_on_ci()) {
  get_java_version()
}
```
