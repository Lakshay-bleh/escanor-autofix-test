# escanor-autofix-test

Test-only repo for Escanor's auto-fix proof scenarios (S1-S8). `scenario/base` is the known-good state; `main` is
broken on purpose by `deploy-ops/autofix-proof/scenarios/*/break.sh` and restored by `reset.sh`. Do not use for real work.

Vercel test app (scenario S4): its build (`build.js`, kept outside this repo) needs the production environment
variable `API_URL` on Vercel project `escanor7/escanor-autofix-vercel`. If the build fails with
"environment variable API_URL is not set", add `API_URL` in that project's settings and redeploy; nothing in this repo changes.
