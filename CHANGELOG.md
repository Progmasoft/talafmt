<!-- SPDX-FileCopyrightText: 2026 Progmasoft <support@progmasoft.com> -->
<!-- SPDX-License-Identifier: MPL-2.0 WITH AdditionRef-Progmasoft-Exception-1.1 -->

# Changelog

## Unreleased

## 0.1.0 - 2026-10-18

The first release of talafmt from a repository of its own. Until now talafmt
lived in the Tala repository, last as version 0.2.0; it moved with its history
and starts its own numbering.

- talafmt is built with the compiler of Tala 0.1.0 through `tala-tooling`,
  pinned to the `tala-0.1.0` commit of Progmasoft/tala until the compiler
  packages are on Hackage.
- `talafmt` formats in place, `--check` reports what would change, and
  `--emit=files|stdout|coverage|checkstyle|json` chooses the output. The
  command line is read by a typed parser written by hand.
- `talafmt.kts` configures the formatter, including the input and output
  encoding and the byte-order mark; the `talafmt-config` helper evaluates it.
