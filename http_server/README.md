# HTTP Server Example

A small web server built on GlowLang's built-in `http` module (`http.listen`, `http.accept`,
`http.read`, `http.send`). An `App` blueprint keeps a table of routes; each route is a function
that returns the response text. Unknown paths get a 404.

```bash
glowlang run app.glow
```

Then open <http://localhost:8080/> and <http://localhost:8080/hello>, or:

```bash
curl http://localhost:8080/hello
```

The server handles one request at a time and runs until you stop it with Ctrl+C. To make HTTP
*requests* from GlowLang, use the [`http` package](https://github.com/anshumali19/GlowLang-packages/tree/main/packages/http).
