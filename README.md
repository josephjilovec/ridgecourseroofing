# True Peak Roofing

A Phoenix homeowner’s field guide from a Summit Hill Holdings venture in development. The public site explains roof materials, helps readers compare proposals and produces a printable or downloadable worksheet. It currently accepts general questions through the studio.

## Run it locally

From this repository on Windows, run the following command and open **http://localhost:8000**.

```powershell
python -m http.server 8000 --directory site
```

On macOS or Linux, use `python3` if that is the installed command. The site is plain HTML, CSS and JavaScript. No account, package installation or backend is required. The material and estimate sections work with JavaScript disabled. The worksheet stays in the browser tab. The plain-text checklist also works offline once downloaded.

## Publish and maintain

`site/` is the complete deployable directory. The Summit Hill Holdings website serves a pinned copy at [the roof guide](https://summithillholdings.com/roofing). Its portfolio entry is [True Peak Roofing](https://summithillholdings.com/portfolio/true-peak-roofing). To update that copy, follow the roofing sync command in the Summit Hill Holdings README. The same site directory can be served directly by a static web host.

Keep service availability and license language consistent across the homepage, terms and portfolio. The images are original AI-generated illustrations of a desert roofscape and three roofing materials. No customer projects are pictured. Responsive WebP files and the locally served Barlow Condensed typeface keep page loads independent of third-party media hosts. Its OFL notice is included under `site/assets/`.
