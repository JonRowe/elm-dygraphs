# Dygraphs in Elm

This package provides component to render [dygraphs] charts.

[dygraphs]: https://github.com/danvk/dygraphs

Original written by @DenisKolodin at DenisKolodin/elm-dygraphs, upgraded to elm 0.18 by @JonRowe.

## Basic Usage

```elm
content : Html msg
content =
  Dygraphs.toHtml
    [ Dygraphs.labels
      [ "X"
      , "Label A"
      , "Label B"
      ]
    , Dygraphs.data <| Dygraphs.Rows [ [1, 3, 6], [2, 34, -1] ]
    ] []
```

Important: This library not contains `dygraphs` library than you should add it to your `index.html`.
