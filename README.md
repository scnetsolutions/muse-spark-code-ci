# muse-spark-code-ci

This repository adds CI capacity to [RandyNorthrup/muse-spark-code](https://github.com/RandyNorthrup/muse-spark-code). It is not the project's home: issues, pull requests and releases live there.

When a pull request is opened or updated there, its commit is pushed here to a `ci/pr-<number>` branch. Part of the build (`.github/workflows/build.yml`, the `org` part) runs here, and the result is posted back to the pull request as the required check `build / org part`. `main` holds only this file, so no scheduled workflow runs here.
