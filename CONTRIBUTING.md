# Contributing to rai-toolkit

Bug reports and PRs are welcome. For anything substantive, open an
[issue](https://github.com/wandb/rai-toolkit/issues) first.

## Setup

```bash
python -m venv .venv && source .venv/bin/activate
pip install -e ".[all]"
```

## Pull request guidelines

- One change per PR.
- Cover behavioural changes with a test.

## Claiming an issue

- Check the issue thread for an existing claim or linked PR before you start.
- To claim, comment on the issue that you're working on it, then open your PR when ready. No need to wait for a reply.
- One PR per issue. When duplicates land, the PR from whoever claimed first gets the review.
- AI-assisted contributions are fine. Say so in the PR description, and be ready to explain and rework any line when asked.

## License headers
<!--- REUSE-IgnoreStart -->

Every source file carries an SPDX header reflecting:
- Year and copyright owner
- SPDX license identifier: `SPDX-License-Identifier: Apache-2.0`
- Package name: `SPDX-PackageName: rai-toolkit`

This is automated with [FSFE REUSE](https://reuse.software/dev/#tool) using the
template in `.reuse/templates/`:

```shell
reuse annotate --license Apache-2.0 --copyright 'CoreWeave, Inc.' --year 2026 \
--template default_template --merge-copyrights $FILE
```

Do not blindly add headers to every file. Assigning the wrong copyright owner
is a real risk. Understand who owns a contribution before annotating it.

Licensing state and the SPDX bill of materials can be validated and generated
with:

```shell
reuse lint
reuse spdx
```

By submitting a contribution you agree it is licensed under Apache-2.0 (see
`LICENSE`).

<!--- REUSE-IgnoreEnd -->

## Security issues

Email **contact@wandb.ai** privately. Don't open a public issue for
vulnerabilities.

## Quick start for new contributors

- Scoped starter work lives under the [good first issue](https://github.com/wandb/rai-toolkit/labels/good%20first%20issue) label.
- Framework mappings (ISO/IEC 42001 #6, Colorado AI Act #7, NYC LL144 #8) mirror the existing NIST AI RMF mapping structure in `rai_toolkit/compliance/`.
- The example policy pack under `rai_toolkit/policies/packs/example_enterprise_pack/` shows the policy format.
- Lint policies with `rai policies lint`.
