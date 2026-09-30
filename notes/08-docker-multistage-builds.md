# Docker Multi-stage Builds

Multi-stage builds let you compile/build in one stage with all devDependencies, then `COPY --from=builder` only the final artifacts into a slim runtime image, cutting image size significantly.
