<!---
  Licensed to the Apache Software Foundation (ASF) under one
  or more contributor license agreements.  See the NOTICE file
  distributed with this work for additional information
  regarding copyright ownership.  The ASF licenses this file
  to you under the Apache License, Version 2.0 (the
  "License"); you may not use this file except in compliance
  with the License.  You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

  Unless required by applicable law or agreed to in writing,
  software distributed under the License is distributed on an
  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  KIND, either express or implied.  See the License for the
  specific language governing permissions and limitations
  under the License.
-->

# DataFusion

<img src="https://arrow.apache.org/datafusion/_images/DataFusion-Logo-Background-White.png" width="256" alt="logo"/>

DataFusion is a very fast, extensible query engine for building high-quality data-centric systems in
[Rust](http://rustlang.org), using the [Apache Arrow](https://arrow.apache.org)
in-memory format. [Python Bindings](https://github.com/apache/arrow-datafusion-python) are also available. DataFusion offers SQL and Dataframe APIs, excellent [performance](https://benchmark.clickhouse.com/), built-in support for CSV, Parquet, JSON, and Avro, extensive customization, and a great community.

Here are links to some important information

- [Project Site](https://arrow.apache.org/datafusion)
- [Rust Getting Started](https://arrow.apache.org/datafusion/user-guide/example-usage.html)
- [Rust DataFrame API](https://arrow.apache.org/datafusion/user-guide/dataframe.html)
- [Rust API docs](https://docs.rs/datafusion/latest/datafusion)
- [Rust Examples](https://github.com/apache/arrow-datafusion/tree/master/datafusion-examples)
- [Python DataFrame API](https://arrow.apache.org/datafusion-python/)
- [Architecture](https://docs.rs/datafusion/latest/datafusion/index.html#architecture)

## What can you do with this crate?

DataFusion is great for building projects such as domain specific query engines, new database platforms and data pipelines, query languages and more.
It lets you start quickly from a fully working engine, and then customize those features specific to your use. [Click Here](https://arrow.apache.org/datafusion/user-guide/introduction.html#known-users) to see a list known users.

## Crate features

Default features:

- `compression`: reading files compressed with `xz2`, `bzip2`, `flate2`, and `zstd`
- `crypto_expressions`: cryptographic functions such as `md5` and `sha256`
- `encoding_expressions`: `encode` and `decode` functions
- `regex_expressions`: regular expression functions, such as `regexp_match`
- `unicode_expressions`: Include unicode aware functions such as `character_length`

Optional features:

- `avro`: support for reading the [Apache Avro] format
- `backtrace`: include backtrace information in error messages
- `pyarrow`: conversions between PyArrow and DataFusion types
- `serde`: enable arrow-schema's `serde` feature
- `simd`: enable arrow-rs's manual `SIMD` kernels (requires Rust `nightly`)

[apache avro]: https://avro.apache.org/

## Rust Version Compatibility

This crate is tested with the latest stable version of Rust. We do not currently test against other, older versions of the Rust compiler.

## Contributing to DataFusion

The [developer’s guide] contains information on how to contribute.

[developer’s guide]: https://arrow.apache.org/datafusion/contributor-guide/index.html#developer-s-guide
