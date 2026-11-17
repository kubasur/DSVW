# SCA test fixture

This fixture intentionally pins requests 2.19.1 to exercise dependency scanning.
It is affected by CVE-2018-18074 (GHSA-x84v-xcm2-53pg).
Do not use these dependencies in a deployed application.

Regenerate the locked requirements with Python 3.10:
`uv pip compile --python-version 3.10 --no-header --no-annotate --output-file requirements.txt requirements.in`
