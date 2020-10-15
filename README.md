# Heroku buildpack for Rust & wasm & Trunk (Yew rs)

## Install this buildpack

### Heroku Application
Add https://github.com/dlacreme/heroku-buildpack-trunk.git to your list of buildpacks.

### CLI

If you're creating a new Heroku application, `cd` to the directory containing your code, and run:

```sh
heroku create --buildpack https://github.com/dlacreme/heroku-buildpack-trunk.git
```

This will only work if your application has a `Cargo.toml` and uses `git`. If you want to set a particular name for application, see `heroku create --help` first.

To use this as the buildpack for an existing application, run:

```sh
heroku buildpacks:add --index 1 https://github.com/dlacreme/heroku-buildpack-trunk.git
```

