# {{ .Title }}

{{- with .Params.links }}
{{ range . -}}
- [{{ .label }}]({{ .url }})
{{ end }}

{{ end -}}
{{- $content := .RawContent -}}
{{- $content = replaceRE `(?m)^\{\{<\s*project-links\s*>\}\}\n?` `` $content -}}
{{ $content }}
