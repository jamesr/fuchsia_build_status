# Fuchsia Dashboard

Simple Flutter module to display the Fuchsia build status. This can be built both as an iOS/Android stand-alone Flutter application, or as a module for Fuchsia.

## How to use in a Fuchsia build

1. ```cd $SRC/apps```
2. ```git clone git@github.com:gregsimon/fuchsia_build_status.git dashboard```
3. ```$SRC/packages/gn/gen.py -m default,../../apps/dashboard/misc_build_files/dashboard```
4. ```$SRC/packages/gn/build.py```
5. Run Fuchsia.
6. On the Fuchsia console:
```device_runner --user_shell=dev_user_shell --user_shell_args=--root_module=dashboard```


