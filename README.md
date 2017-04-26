# gina-cookbook-tools

Repo to handle some gina cookbook tools like delivery build files

### usage

For a default cookbook you edit `.delivery/project.toml` and remove all the lines and leave behind just:

```
remote_file = "https://raw.githubusercontent.com/gina-alaska/gina-cookbook-tools/master/project.toml"
```
Now you can use `delivery local verify`

You can also do a specific test instead of full verify: `lint`, `unit`, `syntax`, `provision`, `deploy`, and `smoke`

If you run `all` it will do all the tests, including the `cleanup`, which will do a `kitchen destroy` as last step.
