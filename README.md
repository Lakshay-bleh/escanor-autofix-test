# escanor-autofix-test

Test-only repo for Escanor's auto-fix proof scenarios (S1-S8). `scenario/base` is the known-good state; `main` is
broken on purpose by `deploy-ops/autofix-proof/scenarios/*/break.sh` and restored by `reset.sh`. Do not use for real work.
