+++
title = "{{ replace .Name "-" " " | title }}"
date = "{{ .Date }}"

# description = "An optional description"

tags = [{{ range $plural, $terms := .Site.Taxonomies }}{{ range $term, $val := $terms }}"{{ printf "%s" $term }}",{{ end }}{{ end }}]
+++

This is a page about {{ replace .Name "-" " " | title }}.
