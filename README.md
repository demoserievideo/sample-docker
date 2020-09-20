# Sample GitHub Artifacts Docker

![Push Container to Artifacts](https://github.com/demoserievideo/sample-artifact-docker/workflows/Push%20Container%20to%20Artifacts/badge.svg)

This .Net Core Sample Project is a sample using GitHub Artifacts to upload your Docker Container Images.

To Autenticate in GitHub Artifacts, i used the action [azure/docker-login@v1](https://github.com/marketplace/actions/docker-login)
   ```
    - uses: azure/docker-login@v1
      with:
        login-server: docker.pkg.github.com
        username: ${{ secrets.GH_PACKAGES_USER }}
        password: ${{ secrets.GITHUB_TOKEN }}
```
In Password, I using the GITHUB_TOKEN, env variable.
\
