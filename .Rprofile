options(
  digits = 4, servr.daemon = TRUE, formatR.indent = 2,
  blogdown.publishDir = '../rnorm-public', blogdown.yaml.empty = FALSE,
  blogdown.subdir = 'blog'
)

local({
  pandoc_path = Sys.getenv('RSTUDIO_PANDOC', NA)
  if (Sys.which('pandoc') == '' && !is.na(pandoc_path)) Sys.setenv(PATH = paste(
    Sys.getenv('PATH'), pandoc_path,
    sep = if (.Platform$OS.type == 'unix') ':' else ';'
  ))
})
