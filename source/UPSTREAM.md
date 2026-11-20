# Upstream source

## Project details

- Name: Flask
- Maintainer: Pallets
- Repository: https://github.com/pallets/flask
- License: BSD-3-Clause
- License file: `LICENSE.txt`
- Inspected commit: `49943b5a94413a530761350f04e896f76e8d620e`
- Python requirement: `>=3.11`

The commit above is a full 40-character commit ID. Use it rather than the moving `main` branch when reproducing the inspected source snapshot.

## Relevant area inspected

- Implementation: `src/flask/views.py`
- Tests: `tests/test_views.py`

The implementation defines `View` and `MethodView`. The tests cover request-method dispatch, inheritance, decorators, automatic OPTIONS handling, HEAD handling, and view initialization.

## Checkout

```bash
git clone https://github.com/pallets/flask.git
cd flask
git checkout 49943b5a94413a530761350f04e896f76e8d620e
```

## License handling

The inspected upstream commit declares BSD-3-Clause in `pyproject.toml` and includes `LICENSE.txt`. If the upstream source is copied or redistributed with this task, retain the original license and copyright notices. Do not replace the upstream license with this repository's own terms.
