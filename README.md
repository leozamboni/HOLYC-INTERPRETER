# HolyC Interpreter

A small sandboxed handwritten HolyC interpreter in JavaScript.

[Playground](https://leonardo.moe/holyc-interpreter/)

If you want a CLI use [HolyC Interpreter CLI](https://github.com/leozamboni/holyc-interpreter-cli).

## Self host

For local run you will need a HTTP server:

```
bun dev
```

Create a input tag with "stdin" tag and another with "stdout/stderr":

```html
<textarea id="stdin"></textarea> 
<textarea id="stdout/stderr"></textarea>
```

The stdin will be for the code and the stdout/stderr for the interpreter output.

Import this procedure in your BOM inside the head tag:

```html
<script defer type="module">
  import { holyc_web_run } from "./holy.js";
  window.holyc_web_run = holyc_web_run;
</script>
```

And call this procedure with a button, for example:

```html
<button onclick="holyc_web_run()">RUN(▶)</button>
```

<hr/>

If you want to support this project star the repository (it makes me motivated ♥).