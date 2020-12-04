FROM registry.redhat.io/ubi8/nodejs-14

USER 0
# Add application sources
ADD . .

RUN chown -R 1001:0 .
USER 1001

# Install the dependencies
RUN npm install

# Run script uses standard ways to run the application
CMD npm run -d start