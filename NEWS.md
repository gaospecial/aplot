# aplot 0.1.10.010

+ prototype of `oncoplot()` (2023-07-18, Tue)
  - with helper functions, `oncoplot_main()`, `oncoplot_sample()` and `oncoplot_gene()`
  - `print()` method for `oncoplot` object
  - `oncoplotGrob()` to convert `oncoplot` object to `grob`
+ control space between subplots (2023-07-15, Sat, #31)
+ `gglistGrob()` to convert a 'gglist' object to a 'gtable' object (2023-06-26, Mon)
+ `<=` to add ggplot component to each of the plots stored in a "gglist" object (2023-06-26, Mon)
+ extend `funky_point()` to support different shapes defined in the 'ggstar' package and extend `funky_bar()` to support grouped bar plot (2023-06-24, Sat, #29)
+ mv `theme_no_margin()` to the 'ggfun' package (2023-06-24, Sat)
+ use `ggfun::theme_blinds()` for funky plots (2023-06-20, Tue)
+ `funky_heatmap()` and relative functions (2023-06-18, Sun)
  + `funky_text()`
  + `funky_point()`
  + `funky_bar()`
+ extend `ggsave()` to support `gglist` object (2023-06-05, Mon, #26)

# aplot 0.1.10

+ fixed R check for a typo in `grid.draw.aplot()` method (2023-03-08, Wed)

# aplot 0.1.9

+ use `ggfun::theme_noxaxis()` instead of `ggtree::theme_dendrogram()` (2022-11-21, Mon)
+ use original scale when sub plot is not a 'ggtree' object (2022-11-18, Fri, #23)

# aplot 0.1.8

+ user can use `options(aplot_align = "y")` to pass the value to `as.patchwork(align="y")` (2022-10-09, Sun)
    - <https://github.com/YuLab-SMU/ChIPseeker/pull/199#pullrequestreview-1135289398>

# aplot 0.1.7

+ `[`, `[<-`, `[[` and `[[<-` methods for the 'aplot' class (2022-08-27, Sat, #22)
+ introduce `align` parameter in `as.patchwork()` (2022-07-27, Wed, #19)

# aplot 0.1.6

+ bug fixed 

# aplot 0.1.5

+ `output` parameter in `plot_list()` can specify to return a `gglist` or `patchwork` object (2022-06-01, Wed)
+ `plot_list()` calls `gglist()` and return a `gglist` object (2022-05-05, Thu)

# aplot 0.1.4

+ `gglist()` function to construct composite plot (2022-05-05, Thu)
+ based on the update of `ggrange()`, now in `xlim2()` and `ylim2()`, we should specify `region = 'plot'` (2022-04-06, Wed)
+ mv `ggrange()`, `xrange()` and `yrange()` to 'ggfun' (2022-04-01, Fri)

# aplot 0.1.3

+ update `ggrange()` to support extracting plot limit and range (newly added) (2022-04-01, Fri)

# aplot 0.1.2

+ bug fixed in setting `plot.tag` theme element in `plot_list` (2021-11-08, Mon) 

# aplot 0.1.1

+ add `labels` parameter in `plot_list` (2021-09-19, Sun)
+ `plot_list` use `ggfun::facet_set()` to use facet label to label subplots (2021-09-17, Fri)
+ `options(aplot_guides = "keep")` to set whether collecting guides (2021-09-16, Thu)
  - <https://github.com/YuLab-SMU/aplot/issues/6#issuecomment-920606540>
+ mv `ggbreak2ggplot`, `is.ggbreak` and `is.ggtree` to the ggfun package and import ggfun
+ `plot_list` now compatible with `ggbreak` object (2021-09-07, Tue)
+ `print(aplot)` will draw the figure and return a `patchwork` object (2021-09-03, Fri; #6)

# aplot 0.1.0

+ add `byrow`, `guides` and `design` parameter in `plot_list`  (2021-09-03, Fri)

# aplot 0.0.9

+ bug fixed for `plot_list` with `patchwork` object (2021-09-03, Fri)
+ `plot_list` supports named plots as input and uses the names as facet labels of the plots  

# aplot 0.0.8

+ update `...`, `tag_levels` and `tag_size` parameters in `plot_list` (2021-09-02, Thu)

# aplot 0.0.7

+ suggest `ggfun` (2021-08-27, Mon)

# aplot 0.0.6

+ `is.ggtree` from treeio package (2020-08-31, Mon)
+ compatible to work with `coord_flip` plot (2020-08-30, Sun)
+ fixed typo (2020-07-24, Fri)

# aplot 0.0.5

+ remove margin in all plots (2020-07-22, Wed)
+ bug fixed of using `insert_*` with `scale_*_discret(limits="")`. (2020-07-03, Fri)
  - <https://github.com/YuLab-SMU/aplot/issues/2>
  - <https://github.com/YuLab-SMU/aplot/pull/3>
+ use `ggplot() + theme_void()` instead of `patchwork::plot_spacer()` for empty plot (2020-04-15, Wed)

# aplot 0.0.4

+ export `xrange` and `yrange` (2020-04-07, Tue)
+ `plot_list` (2020-03-31, Tue)

# aplot 0.0.3

+ CRAN release
  + xlim2()
  + ylim2()
  + insert_left()
  + insert_right()
  + insert_top()
  + insert_bottom()
  + user can use `ggsave` to export the `aplot` object to a figure (e.g. png, pdf)

