# Changelog

# [5.0.0](https://github.com/myii/consul-formula/compare/v4.0.0...v5.0.0) (2020-12-11)


### Bug Fixes

* replace deprecated ui option with ui_config ([b29864a](https://github.com/myii/consul-formula/commit/b29864a1969c2378d5b88f3b2ca8c6a426d034da))


### BREAKING CHANGES

* This cannot be updated in a non-breaking fashion, but
the least disruptive route was chosen.
* If both `ui` and `ui_config.enabled` are set,
`ui_config` takes precedence.  Hence, the change may enable the UI on
machines which had previously set `ui` to false. This is arguably better
than defaulting to `false`, which would disable the UI where it is
supposed to be enabled.
* Removing the option entirely breaks similarly if users
rely on the formula defaults, since Consul's default is `false` and the
formula's default used to be `true`.
* The only other way to break less would be to set both
options, but then users would also have override both (which is not
obvious and very annoying) and there would still be no way forward to
when Consul actually removes the deprecated option.

# [4.0.0](https://github.com/myii/consul-formula/compare/v3.0.0...v4.0.0) (2020-12-11)


### Bug Fixes

* replace deprecated ui option with ui_config ([2223c83](https://github.com/myii/consul-formula/commit/2223c83d1da61e9ca978a0ad0b07a97c23d818f1))


### BREAKING CHANGES

* This cannot be updated in a non-breaking fashion,
but I chose the least disruptive route.

* If both ui and ui_config.enabled are set , ui_config takes precedence.
Hence, my change may enable the UI on machines which had previously set
ui to false. This is arguably better than defaulting to false,
which would disable the UI where it is supposed to be enabled.

* Removing the option entirely breaks similarly if users rely on the formula
defaults, since Consul's default is false and the formula's default used
to be true.

* The only other way to break less would be to set both options, but then
users would also have override both (which is not obvious and very annoying)
and there would still be no way forward to when Consul actually removes the
deprecated option.

# [3.0.0](https://github.com/myii/consul-formula/compare/v2.0.0...v3.0.0) (2020-12-11)


### Bug Fixes

* replace deprecated ui option with ui_config ([f39385d](https://github.com/myii/consul-formula/commit/f39385dd846947aa6e6bb9555859a67b4530451a))


### BREAKING CHANGES

* This cannot be updated in a non-breaking fashion,
but I chose the least disruptive route.
* If both ui and ui_config.enabled are set , ui_config takes precedence.
Hence, my change may enable the UI on machines which had previously set
ui to false. This is arguably better than defaulting to false,
which would disable the UI where it is supposed to be enabled.
* Removing the option entirely breaks similarly if users rely on the formula
defaults, since Consul's default is false and the formula's default used
to be true.
* The only other way to break less would be to set both options, but then
users would also have override both (which is not obvious and very annoying)
and there would still be no way forward to when Consul actually removes the
deprecated option.

# [2.0.0](https://github.com/myii/consul-formula/compare/v1.0.0...v2.0.0) (2020-12-11)


### Bug Fixes

* replace deprecated ui option with ui_config ([feb8570](https://github.com/myii/consul-formula/commit/feb85706ee553f1059a6592525126775cabeaee8))


### BREAKING CHANGES

* This cannot be updated in a non-breaking fashion,
but I chose the least disruptive route.
If both ui and ui_config.enabled are set , ui_config takes precedence.
Hence, my change may enable the UI on machines which had previously set
ui to false. This is arguably better than defaulting to false,
which would disable the UI where it is supposed to be enabled.
Removing the option entirely breaks similarly if users rely on the formula
defaults, since Consul's default is false and the formula's default used
to be true.
The only other way to break less would be to set both options, but then
users would also have override both (which is not obvious and very annoying)
and there would still be no way forward to when Consul actually removes the
deprecated option.

# [1.0.0](https://github.com/myii/consul-formula/compare/v0.13.0...v1.0.0) (2020-12-11)


### Bug Fixes

* replace deprecated ui option with ui_config ([f37b395](https://github.com/myii/consul-formula/commit/f37b395f2799af1f5883181e54e771ac7ff309da))


### BREAKING CHANGES

* This cannot be updated in a non-breaking fashion,
but I chose the least disruptive route.

If both ui and ui_config.enabled are set , ui_config takes precedence.
Hence, my change may enable the UI on machines which had previously set
ui to false. This is arguably better than defaulting to false,
which would disable the UI where it is supposed to be enabled.

Removing the option entirely breaks similarly if users rely on the formula
defaults, since Consul's default is false and the formula's default used
to be true.

The only other way to break less would be to set both options, but then
users would also have override both (which is not obvious and very annoying)
and there would still be no way forward to when Consul actually removes the
deprecated option.

# [0.13.0](https://github.com/myii/consul-formula/compare/v0.12.0...v0.13.0) (2020-12-11)


### Continuous Integration

* **gemfile.lock:** add to repo with updated `Gemfile` [skip ci] ([cdf1565](https://github.com/myii/consul-formula/commit/cdf15658c1a8068a72f2110ede5219c4b4953677))
* **kitchen:** use `saltimages` Docker Hub where available [skip ci] ([0525720](https://github.com/myii/consul-formula/commit/0525720080bfd4fe89e1a84729e31e4055e92b95))
* **kitchen+travis:** add new platforms [skip ci] ([e0e19d5](https://github.com/myii/consul-formula/commit/e0e19d5ea05a029627b0f3aa3516bf9e9b480de3))
* **kitchen+travis:** adjust matrix to add `3000.2` & remove `2018.3` [skip ci] ([5379660](https://github.com/myii/consul-formula/commit/537966061de97cd2ea875fa3986b22e78ac17109))
* **kitchen+travis:** adjust matrix to add `3000.3` [skip ci] ([2d02fdf](https://github.com/myii/consul-formula/commit/2d02fdfdc1725d3f8ef04e2228b8f5965254e69c))
* **kitchen+travis:** adjust matrix to update `3000` to `3000.1` ([d36521c](https://github.com/myii/consul-formula/commit/d36521c262801a6e292b86e783d0d415090e3fa2))
* **kitchen+travis:** remove `master-py2-arch-base-latest` [skip ci] ([f61fd0f](https://github.com/myii/consul-formula/commit/f61fd0f0893d9a0e5cf3ef55155d464c0c40a9bd))
* **pre-commit:** add to formula [skip ci] ([b587c20](https://github.com/myii/consul-formula/commit/b587c20dc91dd5fab36bfe06df27db5812b86288))
* **pre-commit:** enable/disable `rstcheck` as relevant [skip ci] ([1911fa8](https://github.com/myii/consul-formula/commit/1911fa869a3943a33bfa06519e3844cd99b38936))
* **pre-commit:** finalise `rstcheck` configuration [skip ci] ([3bd7a05](https://github.com/myii/consul-formula/commit/3bd7a05d0b4e0b75af82115be2d1789e3c1887f1))
* **travis:** add notifications => zulip [skip ci] ([785955c](https://github.com/myii/consul-formula/commit/785955c10b5e2945ef0aba10742d7a498b5467c3))
* **workflows/commitlint:** add to repo [skip ci] ([2a7adf5](https://github.com/myii/consul-formula/commit/2a7adf5847dcbb227edf2fb20997755190aa10cf))


### Features

* **gitlab-ci:** use GitLab CI as Travis CI replacement ([bcc1d77](https://github.com/myii/consul-formula/commit/bcc1d777efeb6a4fdcf2029a57db7a6ac304c8f6))

# [0.12.0](https://github.com/saltstack-formulas/consul-formula/compare/v0.11.2...v0.12.0) (2020-03-26)


### Features

* **semantic-release:** implement for this formula ([ec8f6c9](https://github.com/saltstack-formulas/consul-formula/commit/ec8f6c92aa91d2714287b640f5210ff62e063ade))
