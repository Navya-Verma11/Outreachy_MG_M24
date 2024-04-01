# Pain Point: Incorrect URL for Boost Download in Ubuntu 18.04 Dockerfile

## Description
During the installation process of FLINT on Ubuntu 18.04 using Docker containers, a significant pain point was encountered. The Dockerfile used to build the base Ubuntu 18.04 container included a URL for downloading Boost libraries that had become outdated and retired, leading to build failures. This issue was documented and tracked as Issue [112](https://github.com/moja-global/FLINT/issues/112).

## Solution Implemented

### Steps Taken
1. **Identification of the Problem:** Upon encountering the build failure, I investigated the issue and identified that the URL for downloading Boost libraries in the Dockerfile was incorrect and outdated.

2. **Research and Alternative Solution:** I researched alternative sources for downloading Boost libraries that were currently being served and identified the Jfrog repository as a viable option.

3. **Modification of Dockerfile:** I edited the Dockerfile to replace the outdated URL with the Jfrog-based URL for downloading Boost libraries. This involved updating the relevant line(s) in the Dockerfile to point to the new URL.

4. **Testing and Validation:** After making the necessary modifications, I rebuilt the Docker container to ensure that the changes were successful and resolved the build failure. The updated Dockerfile resulted in the successful building of the base Ubuntu 18.04 container in Docker without any errors.

5. **Raised a Pull Request:** Finally, I documented the solution implemented and raised a [pull request](https://github.com/moja-global/FLINT/pull/129)

