.PHONY: lint
lint:
	uvx ruff check . --fix

.PHONY: fix
fix:
	uvx ruff format .

.PHONY: test
test:
	pytest .

# Github Actions
.PHONY: lint-check
lint-check:
	uvx ruff check --output-format=github .

.PHONY: format-checkw
format-check:
	uvx ruff format --check .
