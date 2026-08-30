# Internal function to extract the tracelog filename for a BEAST2 input file

Extract the tracelog filename for a BEAST2 input file

## Usage

``` r
extract_tracelog_filename_from_beast2_input_file(input_filename)
```

## Arguments

- input_filename:

  the name of a BEAST2 input XML file. This file usually has an `.xml`
  extension. Use
  [create_temp_input_filename](https://docs.ropensci.org/beastier/reference/create_temp_input_filename.md)
  to create a temporary filename with that extension.

## Value

the name of the tracelog file

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
if (beautier::is_on_ci())
{

  beast2_input_filename <- get_beastier_tempfilename()
  tracelog_filename <- get_beastier_tempfilename()
  beautier::create_beast2_input_file_from_model(
    input_filename = beautier::get_beautier_path("test_output_0.fas"),
    output_filename = beast2_input_filename,
    inference_model = beautier::create_inference_model(
      mcmc = beautier::create_mcmc(
        tracelog = beautier::create_tracelog(
          filename = tracelog_filename
        )
      )
    )
  )
  extract_tracelog_filename_from_beast2_input_file(
    input_filename = beast2_input_filename
  )
  file.remove(beast2_input_filename)

  remove_beaustier_folders()
}
```
