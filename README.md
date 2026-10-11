# AI Workforce Readiness course site

**AI Workforce Readiness: Practical Skills for Work** is a six-week course in practical, responsible use of AI at work.

Visit the live course: <https://hodgkinr.github.io/bobpe-course-site-ai-workforce/>

## Course contents

- Six weekly modules with 12 lectures and 12 readings.
- Six applied activities, six interactive quizzes, and a final project.
- Thirteen local illustrations.
- Four runtime themes: Generic, CU Boulder, Colorado State, and Minnesota Carlson.
- Embedded views using `?embed=1`; for example, <https://hodgkinr.github.io/bobpe-course-site-ai-workforce/modules/week-1/week-1-quiz/?embed=1&theme=cu-boulder>.

Theme choices are available from the page selector and can also be shared in a URL with `?theme=generic`, `?theme=cu-boulder`, `?theme=colorado-state`, or `?theme=minnesota-carlson`. The selected theme follows course navigation. Quizzes are scored in the browser; answers and attempts are not sent to a server.

## Deployment

GitHub Actions deploys the reviewed files in `site/` to GitHub Pages when files under `site/` are pushed to `main`. A manual deployment can be started with the workflow's `workflow_dispatch` option. Documentation-only changes do not start a deployment. The workflow deploys the generated site as-is and does not build or fetch course source material.

## Local preview

From this repository, run:

```sh
python3 -m http.server 8765 --bind 127.0.0.1 --directory site
```

Then open <http://127.0.0.1:8765/index.html>.

## Permissions

Course materials are All Rights Reserved. Reuse requires prior written permission; see [LICENSE.md](LICENSE.md) for details.
