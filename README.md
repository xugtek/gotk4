# gotk4

[![built with nix](https://builtwithnix.org/badge.svg)](https://builtwithnix.org)

A GTK4 bindings generator for Go.

[Package documentation](https://pkg.go.dev/github.com/diamondburned/gotk4/pkg) |
[Package examples](https://github.com/diamondburned/gotk4-examples) |
[GIR documentation](https://pkg.go.dev/github.com/diamondburned/gotk4/gir) |
[Progress tracker](https://github.com/diamondburned/gotk4/issues/2)

All generated packages are in `pkg/`. The generation code is in `gir/girgen/`.

Examples are put in another repository,
[diamondburned/gotk4-examples](https://github.com/diamondburned/gotk4-examples),
along with instructions on getting started with using these packages. Refer to
its README for more information.

As of the time this README was written, most of `pkg/gtk/v4` and `pkg/gtk/v3`
are ready to be used for most purposes. However, memory leaks and sometimes
crashes may occur in certain parts of the API, while other parts might be
completely missing. In that case, an issue should be opened.

## Contributing to gotk4

For contributing guidelines, see [CONTRIBUTING.md](./CONTRIBUTING.md).

## Community

For questions and discussions, join the [**gotk4 Matrix
room**](https://matrix.to/#/#gotk4:matrix.org)!

## License

`gotk4` contains 3 directories licensed differently:

- `gotk4/gir` is licensed under the [GNU Affero General Public License v3][AGPLv3].
  This license does not apply to the code generated by itself.
- `gotk4/pkg` is licensed under the [Mozilla Public License v2][MPLv2].
- `gotk4/pkg/cairo` is licensed under the [MIT license][MIT], originally written
  by "Conformal Systems", later maintained by the [gotk3][gotk3] organization.

[AGPLv3]: https://www.gnu.org/licenses/agpl-3.0.en.html
[MPLv2]: https://www.mozilla.org/en-US/MPL/
[MIT]: https://opensource.org/licenses/MIT
[gotk3]: https://github.com/gotk3/gotk3

Some small snippets of code were taken from
[tinyzimmer's go-glib](https://github.com/tinyzimmer/go-glib), which implements
type subclassing.
