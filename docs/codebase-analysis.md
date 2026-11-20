# Codebase notes

## What Flask does

Flask is a Python web application framework. A Flask application maps URLs to view functions. When a request reaches a URL, Flask calls the associated view and turns its return value into an HTTP response.

## Snapshot examined

- Upstream: https://github.com/pallets/flask
- Commit: `49943b5a94413a530761350f04e896f76e8d620e`
- License: BSD-3-Clause
- Python: `>=3.11`

## Area examined: class-based views

### `src/flask/views.py`

This file defines two main classes:

- `View` provides a base class. A subclass implements `dispatch_request`.
- `MethodView` maps HTTP methods to methods on the Python class. For example, a GET request can call `get`, and a POST request can call `post`.

The `as_view` class method turns a class into a callable view that can be registered with a URL rule.

### `tests/test_views.py`

The corresponding tests cover:

- Basic class-based views.
- Method-based dispatch.
- Replacing the class attached to a generated view.
- Inheritance and multiple inheritance.
- Decorators.
- Automatic OPTIONS behaviour.
- HEAD behaviour.
- Explicit method lists.
- Reusing one view instance across requests.

## Task selection status

This inspection is background work, not evidence of a defect. No bug or missing behaviour has been confirmed yet. A task must be selected only after a concrete expected behaviour and a testable gap have been identified.
