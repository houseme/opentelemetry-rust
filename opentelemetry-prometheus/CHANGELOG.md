# Changelog

## vNext

## 0.29.1

Released 2025-April-11

- Update `prometheus` dependency version to 0.14
- Remove `protobuf` dependency

## v0.29.0

- Update `opentelemetry` dependency version to 0.29
- Update `opentelemetry_sdk` dependency version to 0.29
- Update `opentelemetry-semantic-conventions` dependency version to 0.29

## v0.28.0

- Update `opentelemetry` dependency version to 0.28
- Update `opentelemetry_sdk` dependency version to 0.28
- Update `opentelemetry-semantic-conventions` dependency version to 0.28
- Bump msrv to 1.75.0.

## v0.27.0

- Update `opentelemetry` dependency version to 0.27
- Update `opentelemetry_sdk` dependency version to 0.27
- Update `opentelemetry-semantic-conventions` dependency version to 0.27

## v0.17.0

### Changed

- Update `opentelemetry` dependency version to 0.24
- Update `opentelemetry_sdk` dependency version to 0.24
- Update `opentelemetry-semantic-conventions` dependency version to 0.16

## v0.16.0

### Added

- Add `ResourceSelector` to allow attaching resource as attributes to metrics [#1608](https://github.com/open-telemetry/opentelemetry-rust/pull/1608)

### Changed

- Update `opentelemetry` dependency version to 0.23
- Update `opentelemetry_sdk` dependency version to 0.23

## v0.15.0

### Changed

- Omit empty `otel_scope_info` and `otel_target_info` metrics [#1428](https://github.com/open-telemetry/opentelemetry-rust/pull/1428)

## v0.14.1

### Fixed

- Fix UCUM annotation escaping by ignoring unknown instrument units and annotations [#1348](https://github.com/open-telemetry/opentelemetry-rust/pull/1348)

## v0.14.0

### Changed

- Bump MSRV to 1.65 [#1318](https://github.com/open-telemetry/opentelemetry-rust/pull/1318)
- allow custom units in prometheus suffix [#1188](https://github.com/open-telemetry/opentelemetry-rust/pull/1188)
- Bump MSRV to 1.64 [#1203](https://github.com/open-telemetry/opentelemetry-rust/pull/1203)

## v0.13.0

### Added

- Add `with_namespace` option to exporter config.
- Add more units conversions between OTEL metrics and prometheus metrics [#1157](https://github.com/open-telemetry/opentelemetry-rust/pull/1157).
- Add `without_counter_suffixes` option to exporter config.

### Changed

- Update to opentelemetry-api v0.20.0

## v0.12.0

### Changed

- [Breaking] Add `_total` suffix for all counters [#952](https://github.com/open-telemetry/opentelemetry-rust/pull/952).
- Update to `opentelemetry` v0.19.
- Bump MSRV to 1.57 [#953](https://github.com/open-telemetry/opentelemetry-rust/pull/953).
- Update dependencies and bump MSRV to 1.60 [#969](https://github.com/open-telemetry/opentelemetry-rust/pull/969).
- Add `otel_scope_info` and `scope` labels [#974](https://github.com/open-telemetry/opentelemetry-rust/pull/974).

## v0.11.0

### Changed

- Update to opentelemetry v0.18.0

### Removed

- BREAKING: `PrometheusExporter::new()` removed. Use `ExporterBuilder`. #727

## v0.10.0

### Added

- Added `prometheus-encoding` feature to export prometheus encoders #652
- Added `with_aggregator_selector` option #667

### Changed

- Update prometheus to 0.13 #644
- Update to opentelemetry v0.17.0

### Fixed

- Enable directly constructing a SpanExporter #655

## v0.9.0

### Added

- Add `from_env` to prometheus exporter builder #605
- Adds `Default` implementation to `ExporterBuilder` based on the otel specification environment variables #242

### Changed

- Update to opentelemetry v0.16.0

### Deprecated

- `PrometheusExporter::new()` is deprecated in favor of using `ExporterBuilder`

## v0.8.0

### Changed

- Update to opentelemetry v0.15.0

## v0.7.0

### Changed

- Update to opentelemetry v0.14.0

## v0.6.0

### Added

- Add sanitization of prometheus label names #462

### Changed

- Update to opentelemetry v0.13.0
- Update prometheus dependency #485

## v0.5.0

### Added

- Batch observer support #429

### Changed

- Update to opentelemetry v0.12.0
- Update tokio to v1 #421
- Update prometheus to v0.11 #435

## v0.4.0

### Changed

- Update to opentelemetry v0.11.0
- Add non monotonic counter support #385

## v0.3.0

### Changed

- Update to opentelemetry v0.10.0

## v0.2.0

### Changed

- Update to prometheus 0.10.x #279

## v0.1.0

### Added

- Initial prometheus exporter
