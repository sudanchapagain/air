+++
title = "{{ replace .Name "-" " " | title }}"
date = "{{ .Date }}"

# Set menu to "main" to add this page to the main menu on top of the page
menu = "main"

# description = "An optional description"

# tags are optional
# tags = [{{ range $plural, $terms := .Site.Taxonomies }}{{ range $term, $val := $terms }}"{{ printf "%s" $term }}",{{ end }}{{ end }}]
+++

This is a page about {{ replace .Name "-" " " | title }}.
