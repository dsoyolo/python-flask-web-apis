# python-flask-web-apis

<https://programminghistorian.org/en/lessons/creating-apis-with-python-and-flask>

Other:
Prettify JSON output such as SARIF compliant tools

Command-line tool to validate and pretty-print JSON
<https://github.com/python/cpython/blob/3.9/Lib/json/tool.py>

Usage:

```bash
$ echo '{"json":"obj"}' | python -m json.tool
{
    "json": "obj"
}
```

When using semgrep, run:

```bash
semgrep --config s/ubimars:flask-debug-enabled --sarif api/api_final.py | python3.9 -m json.tool > output/sarif-output.json
```
