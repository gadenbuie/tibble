# output test

    Code
      rownames_to_column(mtcars, "cyl")
    Error <tibble_error_column_names_must_be_unique>
      Column name `cyl` must not be duplicated.
      Caused by error in `stop_vctrs()`:
      ! Names must be unique.
      x These names are duplicated:
        * "cyl" at locations 2 and 12.
    Code
      rowid_to_column(trees, "Volume")
    Error <tibble_error_column_names_must_be_unique>
      Column name `Volume` must not be duplicated.
      Caused by error in `stop_vctrs()`:
      ! Names must be unique.
      x These names are duplicated:
        * "Volume" at locations 3 and 4.
    Code
      column_to_rownames(mtcars, "cyl")
    Error <tibble_error_already_has_rownames>
      `.data` must be a data frame without row names.
    Code
      column_to_rownames(trees, "foo")
    Error <tibble_error_unknown_column_names>
      Can't find column `foo` in `.data`.

