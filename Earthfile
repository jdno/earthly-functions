VERSION 0.8
PROJECT jdno/earthly-functions

format-json:
    ARG FIX="false"
    DO ./prettier+PRETTIER --EXTENSION="json" --FIX="$FIX"

format-markdown:
    ARG FIX="false"
    DO ./prettier+PRETTIER --EXTENSION="md" --FIX="$FIX"

format-yaml:
    ARG FIX="false"
    DO ./prettier+PRETTIER --EXTENSION="{yaml,yml}" --FIX="$FIX"

# lint-markdown checks Markdown files for linting errors
lint-markdown:
    DO ./markdown+LINT

# lint-yaml checks YAML files for linting errors
lint-yaml:
    DO ./yaml+LINT

prettier:
    ARG FIX="false"
    DO ./prettier+PRETTIER --FIX="$FIX"
